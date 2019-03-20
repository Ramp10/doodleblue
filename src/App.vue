<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <div class="container-fluid">
        
          <div class="row"> 
              <div class="bg-gradient left-bar" > 
                  <p class="text-center mt-3"><img class="alert-icon" alt="alert-icon" src="./assets/baseline-offline_bolt-24px.svg">  </p>
                  <ul class="nav nav-pills flex-column margin-top--icons text-center"> 
                      <li class="nav-item"> 
                        <a class="nav-link active" data-toggle="pill"> 
                          <img class="alert-icon" alt="alert-icon" src="./assets/baseline-supervised_user_circle-24px.svg"> 
                         </a> 
                      </li>
                      <li class="nav-item"> 
                        <a class="nav-link" data-toggle="pill"> 
                          <img class="alert-icon" alt="alert-icon" src="./assets/baseline-import_contacts-24px.svg"> 
                         </a> 
                      </li>
                  </ul>
              </div>
          <router-view/>
        </div>
        
        
    </div>

    
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /*margin-top: 60px;*/
}

.bg-gradient{
  /* Permalink - use to edit and share this gradient: http://colorzilla.com/gradient-editor/#fd8465+1,ff7980+27,ff699c+100,bef2ff+100 */
background: #fd8465; /* Old browsers */
background: -moz-linear-gradient(top, #fd8465 1%, #ff7980 27%, #ff699c 100%, #bef2ff 100%); /* FF3.6-15 */
background: -webkit-linear-gradient(top, #fd8465 1%,#ff7980 27%,#ff699c 100%,#bef2ff 100%); /* Chrome10-25,Safari5.1-6 */
background: linear-gradient(to bottom, #fd8465 1%,#ff7980 27%,#ff699c 100%,#bef2ff 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#fd8465', endColorstr='#bef2ff',GradientType=0 ); /* IE6-9 */

}
.left-bar{
  height: 100vh;
width:60px !important;

}

.nav-link.active{
  color: #fff;
    background-color: transparent !important;
    border-left-color: #fff;
    border-left: 3px solid;
    border-radius:0px !important;
}


</style>
