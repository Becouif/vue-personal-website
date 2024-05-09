<script setup>
import '../assets/css/portfolio.css'
</script>
<template>
        <section class="portfolio" id="portfolio">
         <div class="container">
            <div class="row">
               <div class="title text-center">
                  <h1>Latest Works</h1>
               </div>
            </div>
            <!-- <div class="row">
               <div class="filter-btn">
                  <ul id="filterBtn">
                     <li class="active" data-target="all">All</li>
                     <li data-target="web">Full Stack development</li>
                     <li data-target="app">Front end Development/ UI/UX</li>
                     <li data-target="ui">Backend Development</li>
                  </ul>
               </div>
            </div> -->
            <div class="row text-center">
               <div class="gallery">
                  <a class="item-link" href="">
                     <div class="item" data-id="web">
                        <div class="inner">
                           <img src="../assets/img/portfolio/cuisine-share.png" alt="cuisine-share"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>

                              <h4>Cuisine Share</h4>
                           </div>
                        </div>
                     </div>
                  </a>
                  <a class="item-link" href="">
                     <div class="item" data-id="web">
                        <div class="inner">
                           <img src="../assets/img/portfolio/monstergame.png" alt="monster game"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>
                              <h4>Web Design</h4>
                           </div>
                        </div>
                     </div>
                  </a>
                  <a class="item-link" href="">
                     <div class="item" data-id="app">
                        <div class="inner">
                           <img src="../assets/img/portfolio/movie-series-overview.png" alt="movie overview"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>
                              <h4>App Interface</h4>
                           </div>
                        </div>
                     </div>
                  </a>
                  <a class="item-link" href="">
                     <div class="item" data-id="app">
                        <div class="inner">
                           <img src="../assets/img/portfolio/vue-id-card-maker.png" alt="ID Card"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>
                              <h4>App Interface</h4>
                           </div>
                        </div>
                     </div>
                  </a>
                  <a class="item-link" href="">
                     <div class="item" data-id="ui">
                        <div class="inner">
                           <img src="../assets/img/portfolio/ui2.png" alt="portfolio"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>
                              <h4>UI/UX Design</h4>
                           </div>
                        </div>
                     </div>
                  </a>
                  <a class="item-link" href="">
                     <div class="item" data-id="ui">
                        <div class="inner">
                           <img src="../assets/img/portfolio/ui3.png" alt="portfolio"/>
                           <div class="overlay">
                              <span class="fa fa-plus"></span>
                              <h4>UI/UX Design</h4>
                           </div>
                        </div>
                     </div>
                  </a>
               </div>
            </div>
         </div>
      </section>
</template>