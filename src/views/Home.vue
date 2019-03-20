<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <Index msg="Welcome to Your Vue.js App"/> -->

    <!-- Header -->
      <div class="row home-header py-2"> 
      
        <div class="col-sm-7 float-left"> 
          <span> 
            <img  class="search-icon" alt="search-icon" src="../assets/baseline-search-24px.svg">
          </span>
        </div>
        <div class="col-sm-5 pt-2"> 
            <div class="row text-right">
              <div class="col-sm-3 font-weight-bold"> <span class="cursor"> + Add </span> </div>
              <div class="col-sm-2"> 
                <span class="cursor"> 
                  <img class="mail-icon" alt="mail-icon" src="../assets/baseline-mail_outline-24px.svg">   
                </span>
              </div>
              <div class="col-sm ">
                  <select class="select-opt font-weight-bold">
                      <option> Mark1</option>
                      <option> Mark2</option>
                      <option> Mark3</option>
                  </select>

              </div>
              <div class="col-sm-2">
                <span class="cursor"> 
                  <img class="alert-icon" alt="alert-icon" src="../assets/outline-notification_important-24px.svg">  
                </span>
              </div>
            </div>
        </div> 
      
      </div>
    <!-- Header Close -->

    
        <div class="row px-5 pt-4 pb-2"> 
            <span>
              <img class="contact-icon bg-gradient" src="../assets/baseline-contacts-24px.svg"  width="40" alt="contact-book"> 
            </span>
            <div class="col-sm-4"> 
               
                <h3>Contacts </h3>
                 <span> contacts page data </span>
            </div>
        </div>

        <div class="row  px-4 py-3"> 
            <div class="col-sm-12"> 
              <span class="search-icon p-3">
                <input type="text" v-model="searchText" class="input-search" placeholder="Search contacts" > 
                <img alt="search-icon" src="../assets/baseline-search-24px.svg">
              </span>

                            <button class="bg-gradient btn-contact--add"> + Add Contact </button>
            </div>

        </div>
        <div class="row px-5 py-3"> 
          <div class="col-sm-6 contact-list">
            <contacts/> </div>

            <div class="col-sm-6 view-list"> 
                <userView />
            </div>
        </div>
        
  </div>
</template>

<script>
// @ is an alias to /src
import Index from '@/components/index.vue'
import contacts from "@/components/contacts.vue"
import userView from "@/components/userView.vue"
export default {
  name: 'home',
  components: {
    Index,
    contacts,
    userView
  },
  data(){
    return{
      searchText: ""
    }
  }
}
</script>

<style scoped> 
.row{
  margin:0px;
}
  .cursor{
    cursor: pointer;
  }
  .home{
    width: calc(100% - 60px);
     height: 100vh;
      
  }

  .search-icon{
    background: #ddd;
     margin: 5px 25px;
    padding: 5px;
    border-radius:25px;
  }
  .home-header{
    border-bottom: 1px solid #ddd;
    margin:0px;
  }

  .select-opt{
    border: 0px;
    width: 100px;
    outline: none;
  }

  .input-search{
    border: transparent;
    background: transparent;
    outline: none;
    margin:5px;
    padding:10px;
  }

  .btn-contact--add{
    border: 0px;
    padding: 13px 20px;
    border-radius: 5px;
    font-weight: 600;
    color: #fff;
    outline:none;
  }
  .contact-icon{
    border-radius: 5px;
  }

  .contact-list{
        overflow: auto;
    height: 380px;
  }

  .view-list{
        padding: 0px 25px;
  }
</style>
