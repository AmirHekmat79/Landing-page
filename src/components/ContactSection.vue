<template>
    <div class="q-pa-md bg-blue-grey-2 "> 
        <div class="row  justify-around   items-center">
            <div class="col-xs-12 col-md-6">
                <h4>Contact Us</h4> 
                <div class="bg-teal-14 divider q-mb-xl"></div>
                <h6>Address</h6>
                <p>Swing by for a cup of coffee, or whatever.</p>
                <p class="text-h6" ><q-icon color="teal-7"  name="place" class="q-mr-md"></q-icon>Chicago, US</p>
                <p class="text-h6" ><q-icon color="teal-7"  name="phone" class="q-mr-md"></q-icon>+00 1515151515</p>
                <p class="text-h6" ><q-icon color="teal-7" name="mail" class="q-mr-md"></q-icon> test@test.com</p>
            </div>    
            <div class="col-xs-12 col-md-6 q-mt-sm ">
              <form>
                <q-card class="my-card shadow-8 bg-white  text-white shadow-transition q-pa-xl">
                <q-card-section class="text-dark column">
                <label for="Name">Name</label>
                <input class="border-style" type="text" id="Name" />
               </q-card-section>
               <q-card-section class="text-dark column">
                <label for="Email">Email</label>
                <input class="border-style" type="text" id="Email" />
               </q-card-section>
              
               <q-card-section class="text-dark column">
                <label for="Message">Message</label>
                <input class="border-style" type="text" id="Message" />
               </q-card-section>
               
               <q-card-actions>
                <div class="q-mr-auto">
                    <input type="checkbox" id="I Like it!" checked />
                    <label class="text-dark" for="I Like it!">I Like it!</label>
                </div>
                   <q-btn type="submit" class="button">Send</q-btn>
               </q-card-actions>
           </q-card>
              </form>
            </div>
        </div>           
     </div>        
              
   
   </template>
<style scoped>
.button{
 border: none;
 cursor: pointer;
 color: #fff !important;
 background-color: #000000 !important;
 padding: 8px 16px;
}
.button:hover{
 background-color: #edeaea !important;
 color : #000000 !important;

}
.border-style{
    border: none;
    border-bottom: 1px solid #ccc;
    width : 100%;
    padding: 8px;
    display: block;
}
.divider{
    border-bottom : 6px solid #009688;
    width : 10rem;
 
}
</style>       
  