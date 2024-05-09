<script setup>
import '../assets/css/blog.css'

</script>
<template>
       <section class="blog" id="blog">
         <div class="container">
            <div class="row">
               <div class="title text-center">
                  <h1>Latest Blogs</h1>
               </div>
            </div>
            <div class="row">
               <div class="blog-content">
                  <div class="blog-box">
                     <div class="blog-img">
                        <!-- <img src='./img/blogs/1.jpg' /> -->
                        <img src="../assets/img/blogs/1.jpg" />
                     </div>
                     <div class="blog-text">
                        <div class="blog-info">
                           <span>May 3, 2020</span>
                           <span>Version Control</span>
                        </div>
                        <h3>Why every developer uses Git.</h3>
                        <p>Git allows us to have a “version” of a project which shows the changes that were made to the code over time, and allows us to backtrack if necessary and undo the changes.</p>
                        <a href="https://devpuskar.netlify.app/blogs/04git">Read More</a>
                     </div>
                  </div>
                  <div class="blog-box">
                     <div class="blog-img">
                        <img src='../assets/img/blogs/2.png' />
                     </div>
                     <div class="blog-text">
                        <div class="blog-info">
                           <span>May 1, 2020</span>
                           <span>Web Development</span>
                        </div>
                        <h3>JavaScript Promises</h3>
                        <p>Before we use promises, our code was full of confusing callback tricks and asynchronous. Switching to promises made our code easier to read, understand, and test.</p>
                        <a href="https://devpuskar.netlify.app/blogs/03jspromises">Read More</a>
                     </div>
                  </div>
                  <div class="blog-box">
                     <div class="blog-img">
                        <img src='../assets/img/blogs/3.jpg' />
                     </div>
                     <div class="blog-text">
                        <div class="blog-info">
                           <span>April 27, 2020</span>
                           <span>Programming</span>
                        </div>
                        <h3>Why we don’t need a degree to be a Developer.</h3>
                        <p>That's right. You don’t need a degree to be a developer. Whilst university is definitely the right path for some people, it is not right for everyone.</p>
                        <a href="https://devpuskar.netlify.app/blogs/01developerdegree">Read More</a>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </section>
</template>