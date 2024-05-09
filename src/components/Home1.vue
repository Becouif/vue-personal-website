<script setup>
import {ref} from 'vue';
import '../assets/css/home.css'
import Home1 from './sub/Download.vue';
const pdfUrl = ref('../assets/cv/blessing-afolabi-full-stack-developer.pdf');
const pdfFileName = ref('blessing-afolabi-file.pdf');
</script>

<template>
  <section class="home" id="home">
         <div class="container">
            <div class="row full-screen">
               <div class="home-content">
                  <div class="block">
                     <h6>Hi, my name is</h6>
                     <h1>Blessing Afolabi</h1>
                     <h3>I build things for the web</h3>
                     <div class="cv-btn">
                      <Home1 :pdf-url="pdfUrl" :pdf-file-name = "pdfFileName" />
                        <!-- <button @click="downloadCV">Download new</button> -->
                        <a href="('../assets/cv/blessing-afolabi-full-stack-developer.pdf')" download="../assets/cv/blessing-afolabi-full-stack-developer.pdf" target="_blank">Donwload CV</a>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </section>
</template>