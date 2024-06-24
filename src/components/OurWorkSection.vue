<template>
<div class="q-pa-md bg-blue-grey-10 text-white q-gutter-sm"> 
    <div class="row  justify-around   items-center  text-justify q-pa-md">
        <div class="col-md-3 col-xs-12 col-sm-6 q-my-sm">
          <h4>Our Work</h4>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>
        <div class="col-md-3 col-xs-12  col-sm-6 q-my-sm q-gutter-x-lg">
            <q-card class="my-card">
        <img src="../assets/snow.jpg" width="100%">

        <q-card-section class="text-dark">
            <div class="text-h5">Customer 1</div>
            <div class="text-h6 q-my-md">Trade</div>
            <div v-for="(n,index) in 4" :key="index" class="text-h6 q-my-xs">Blablabla</div>
        </q-card-section>
    </q-card>

       </div>
       <div class="col-md-3 col-xs-12  col-sm-6 q-my-sm q-gutter-x-lg">
            <q-card class="my-card">
        <img src="../assets/lights.jpg" width="100%">

        <q-card-section class="text-dark">
            <div class="text-h5">Customer 2</div>
            <div class="text-h6 q-my-md">Trade</div>
            <div v-for="(n,index) in 4" :key="index" class="text-h6 q-my-xs">Blablabla</div>
        </q-card-section>

    </q-card>

       </div>
       <div class="col-md-3 col-xs-12  col-sm-6 q-my-sm q-gutter-x-lg">
            <q-card class="my-card">
        <img src="../assets/mountains.jpg" width="100%">

        <q-card-section class="text-dark">
            <div class="text-h5">Customer 3</div>
            <div class="text-h6 q-my-md">Trade</div>
            <div v-for="(n,index) in 4" :key="index" class="text-h6 q-my-xs">Blablabla</div>
        </q-card-section>

    </q-card>

       </div>
    </div>
   
     
</div>
   

</template>

