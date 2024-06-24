<template>
   <div class="q-pa-md  q-gutter-sm"> 
       <div class="text-center">
        <h4>OUR TEAM</h4>
       <h5>Meet the team - our office rats:</h5>
       </div>
    <div class="row justify-center items-center text-center q-pa-md">
        <div class="col-md-3 col-xs-12 col-sm-4" v-for="(n , index) in 4" :key="index">
            <q-img  width="45%" class="rounded-border"   src="../assets/avatar.jpg" />
            <h5 class="q-my-md">Johnny Walker</h5>
            <p>Web Designer</p>
        </div>
    </div>
    
  </div>
</template>

<style scoped>
.rounded-border{
    border-radius: 50%;
}

</style>