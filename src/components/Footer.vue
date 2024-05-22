<script setup>
import '../assets/css/footer.css';
import {ref} from 'vue';
const d = new Date();
let year = d.getFullYear();
let currentYear = ref(year);

</script>
<template>
  <div>
    <footer>
         <div class="container">
            <div class="row">
               <div class="footer-logo">Blessing Afolabi</div>
               <div class="social-link">
                  <a href="https://www.facebook.com/afolabi.enoch2" target="_blank"><i class="fa fa-facebook"></i></a>
                  <!-- <a href=""><i class="fa fa-instagram"></i></a> -->
                  <!-- <a href=""><i class="fa fa-twitter"></i></a> -->
                  <a href="https://www.linkedin.com/in/blessing-afolabi/" target="_blank"><i class="fa fa-linkedin"></i></a>
                  <a href="https://github.com/Becouif" target="_blank"><i class="fa fa-github"></i></a>
               </div>
            </div>
         </div>
      </footer>
      <section class="copyright">
         <div class="container">
            <p> © 2024 - {{currentYear}}<span id="year"></span> | Developed By Blessing Afolabi. | All rights reserved.</p>
         </div>
      </section>
      <div class="lightbox hide">
         <span class="close-lightbox fa fa-close"></span>
         <img src="" alt="portfolio"/>
      </div>
  </div>
</template>