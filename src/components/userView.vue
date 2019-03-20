<template>
<div class="user-card">
    <div class="row ">
        <div class="col-sm-12 text-center"> 
            <p class="p-4 mb-0">
                <span class="user-icon">
                    MH  
                </span>
            </p>
            <p class="user-name font-weight-bold pt-3 pb-1 m-0"> Mike Houston </p>
            <p class="user-role"> product manager </p>

        </div>
    </div>
    <div class="row border-down">
        <div class="col-sm-6"> 
            <!-- Full Name -->
            <p class=""> <span> Full Name:</span> </p> 
        </div>
        <div class="col-sm-6">
         <p class="">  <span class="pl-3"> Mike Houston </span> </p> 
        </div>
    </div>
       <div class="row border-down">
        <div class="col-sm-6"> 
   
             <p class=""> <span> Email:</span>  </p> 

        </div>
        <div class="col-sm-6">
         <p class="">  <span class="pl-3"> Mike Houston </span> </p> 
        </div>
    </div>
       <div class="row border-down">
        <div class="col-sm-6"> 
            <!-- Full Name -->
            <p class=""> <span> Phone:</span>  </p> 
        </div>
        <div class="col-sm-6">
         <p class="">  <span class="pl-3"> Mike Houston </span> </p> 
        </div>
    </div>
       <div class="row border-down">
        <div class="col-sm-6"> 
            <!-- Full Name -->
            <p class=""> <span> Company:</span> </p> 
        </div>
        <div class="col-sm-6">
         <p class="">  <span class="pl-3"> Mike Houston </span> </p> 
        </div>
    </div>    
</div>
</template>

<script>
export default {
    name:"userView",
    data(){
        return {

        }
    },
     computed(){
        
     }

}
</script>

<style scoped>
.row{
  margin:10px;

}

.user-card{
    background: #ddd;
    padding:2px 15px;
}

.user-icon{
    border-radius: 50%;
    padding:25px;
    background: #ccc;
}

.border-down{
    border-bottom: 1px solid #ccc
}
</style>
