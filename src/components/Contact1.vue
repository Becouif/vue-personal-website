<script>
import '../assets/css/contact.css';

</script>
<template>
       <section class="contact" id="contact">
         <div class="container">
            <div class="row">
               <div class="title text-center">
                  <h1>Get In Touch</h1>
               </div>
            </div>
            <div class="row">
               <div class="contact-form">
                  <div class="row">
                     <div class="contact-text">
                        <h2>Drop Me message</h2>
                        <p>My inbox is always open I'll try my best to get back to you!</p>
                     </div>
                  </div>
                  <div class="row space-between">
                     <div class="col-6">
                        <input type="text"  class="form-control" name="name" placeholder="Name" />
                     </div>
                     <div class="col-6">
                        <input type="email" class="form-control" name="email" placeholder="Email" />
                     </div>
                  </div>
                  <div class="row">
                     <div class="col-12">
                        <textarea name="message" class="form-control" placeholder="Your Message"></textarea>
                     </div>
                  </div>
                  <div class="row">
                     <div class="button btn">
                        <!-- <button @click="sendEmail">Get In Touch</button> -->
                        <a href="#">Get In Touch</a>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </section>
</template>