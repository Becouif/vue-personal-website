<script>
import '../assets/css/contact.css';
import emailjs from 'emailjs-com';

export default {
  // name: 'ContactUs',
  data() {
    return {
      name: '',
      email: '',
      message: ''
    }
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm('service_9bqqxl5', 'template_p0sh9m7', '#contact-form',
        'Zyyik1O5V8oP7MoTL', {
          name: this.name,
          email: this.email,
          message: this.message
        })

      } catch(error) {
          console.log({error})
      }
      // Reset form field
      this.name = ''
      this.email = ''
      this.message = ''
    },
  }
}
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

                <form  method="post" id="contact-form">
                    <div class="row space-between">
                      <!-- start  -->



                      <div class="col-6">
                          <input type="text" v-model="name" class="form-control" name="name" placeholder="Name" />
                      </div>
                      <div class="col-6">
                          <input type="email" v-model="email" class="form-control" name="email" placeholder="Your Email" />
                      </div>
                    </div>
                    <div class="row">
                      <div class="col-12">
                          <textarea name="message" v-model="message" class="form-control" placeholder="Your Message"></textarea>
                      </div>
                    </div>
                    <div class="row">
                      <div class="button btn">
                          <a  @click="sendEmail">Get In Touch</a>
                          <!-- <a href="#">Get In Touch</a> -->
                      </div>
                    </div>
                  <!-- end  -->
                </form>
               </div>
            </div>
         </div>
      </section>
</template>