<template>
         <div class="container">
             <div class="row">
                    <div class="home-header">
                            <!--  <img src="../../assets/bg-header.jpg"> -->
                            <p class="enegeize">Enegeize</p>
                   </div>
             </div>
                <router-view></router-view> 
             <div class="row">
                 <app-products></app-products>
             </div>
             <div class="row">
                 <app-features></app-features>
             </div>
             <div class="row">
                <app-dashboard></app-dashboard>
             </div>
             <div class="row">
               <app-gallery></app-gallery>
             </div>
             <div class="row">
               <app-specs></app-specs>
            </div>
         </div>        
 </template>
 
 <script>
 import Header from './header.vue';
 import Products from './content/menuProducts.vue';
 import Features from './content/Features.vue';
 import Dashboard from './content/dashboard.vue';
 import Gallery from './content/Gallery.vue';
 import Specs from './content/Specs.vue';
 
 export default {
     components:{
           'app-header' : Header,
           'app-products' : Products,
           'app-features' : Features,
           'app-dashboard' : Dashboard,
           'app-gallery' : Gallery,
           'app-specs' : Specs
     }
 }
 </script>
 
 <style scoped>
 .enegeize{
     font-size: 110pt;
     color: white
 }
 img{
     width: 100%;
 }
 .home-header{
     width: 100%;
     background-image: url('../../assets/bg-header.jpg');
     text-align: center;
 }
 </style>
 