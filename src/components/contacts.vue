<template>
<div>
    <div class="row px-4 py-3 bg-light border-down">
        <div class="col-sm-1"> 
            +
        </div>
                <div class="col-sm-5 py-4"> 
                    Basic Info
        </div>
                <div class="col-sm-4 py-4"> 
                    Company
        </div>
    </div>
    <div class="row px-4 py-3 bg-light cursor" v-for="user in userData" :key="user.id" @click="selectUser(user)">
        <div class="col-sm-1"> 
            <input type="checkbox">
        </div>
                <div class="col-sm-5"> 
                    <p> {{user.name}} </p>
        </div>
                <div class="col-sm-4"> 
                    <p> {{user.company.name}} </p>
        </div>
    </div>
</div>
</template>

<script>
import axios from 'axios'

export default {
    name: "contacts",
    data(){
        return{
            userData: []
        }
    },

    created(){
        axios(`https://jsonplaceholder.typicode.com/users`)
            .then(res => this.userData = res.data )
            .catch(e => console.err(e))
    },
    methods:{
        selectUser(user){
            this.emit('getUserData', user)
        }
    }

}
</script>

<style scoped>
.row{
  margin:0px;

}
.border-down{
    background: #ddd;
}
  .cursor{
    cursor: pointer;
  }
</style>
