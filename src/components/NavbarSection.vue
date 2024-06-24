<template>
        <q-header class="bg-dark">
         
          <q-toolbar class="navigation-toolbar  q-pa-sm">
            <q-btn class="button q-px-md q-mx-sm" icon="home">Logo</q-btn>
            <q-btn class="bg-dark q-px-md q-mx-sm">Team</q-btn>
            <q-btn class="bg-dark q-px-md q-mx-sm">Work</q-btn>
            <q-btn class="bg-dark q-px-md q-mx-sm">Price</q-btn>
            <q-btn class="bg-dark q-px-md q-mx-sm">Contact</q-btn>
            <q-btn-dropdown class="bg-dark q-px-md q-mx-sm"  label="Dropdown">
              <q-list>
                <q-item clickable v-close-popup >
                  <q-item-section>
                    <q-item-label class="text-subtitle1">Link</q-item-label>
                  </q-item-section>
                </q-item>
                <q-item clickable v-close-popup >
                  <q-item-section>
                    <q-item-label class="text-subtitle1">Link</q-item-label>
                  </q-item-section>
                </q-item>
                <q-item clickable v-close-popup >
                  <q-item-section>
                    <q-item-label  class="text-subtitle1">Link</q-item-label>
                  </q-item-section>
                </q-item>
              </q-list>
            </q-btn-dropdown>
             
            <q-btn class="bg-dark search-icon"  icon="search"></q-btn>
          </q-toolbar>
        
          <q-toolbar  class="row justify-between items-center resDevices" >
            <q-btn class="button" icon="home">Logo</q-btn>
           
            <q-btn class="navigation-menuButton" icon="menu" @click="showMenu"></q-btn>
          </q-toolbar>
          <ul class="column justify-center items-center q-mx-auto text-center list-container" v-if="show">
              <li>
                <q-btn class="bg-dark q-pa-sm">Team</q-btn>
              </li>  
              <li>
                <q-btn class="bg-dark q-pa-sm">Work</q-btn>
              </li>
              <li>
                <q-btn class="bg-dark q-pa-sm">Price</q-btn>
              </li>
                <li>
                  <q-btn class="bg-dark q-pa-sm">Contact</q-btn> 
                </li>
                  <li>
                    <q-btn class="bg-dark q-pa-md">Search</q-btn> 
                  </li>
         
            </ul>
        </q-header>
    
</template>
<script>
export default{
  name : 'NavbarSection' ,
  data(){
    return {

        show : true,
    }
  } ,
  methods:{
    showMenu(){
      if(this.show){
        this.show = false;
      }else{
        this.show = true;
      }
    }
  }
}
</script>
<style scoped> 

.button{
  background-color: #009688 !important;
}
.button:hover{
    cursor: pointer;
    background-color: #edeaeaec !important;
    color : #000000 !important;
}

.list-container{
  list-style-type: none;
  display: none;

}
.search-icon{
  position: absolute;
  right: 0;
}
@media only screen and (max-width: 630px) {
  .navigation-toolbar{
    display : none;
  }
  .navigation-menuButton{
    display : block;
  }
  .list-container{
  display: block;

}
}


@media only screen and (min-width: 631px) {
  .navigation-menuButton{
    display : none;
  }
  .navigation-toolbar{
    display : block;
  }
  .resDevices{
    display: none;
  }
}
</style>