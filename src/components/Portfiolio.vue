<script setup>
import '../assets/css/portfolio.css'

</script>

<template>
<section class="portfolio" id="portfolio">
    <div class="body">
                <div class="title text-center">
                  <h1>Latest Works</h1>
                </div>
    
      <a href="https://laravel-deploy.com" target="_blank" class="card item">
        <div class="card-content">
          <!-- <div class="inner"> -->
            <img class="card-img" src="../assets/img/portfolio/cuisine-share.png" alt="cuisine-share"/>
            <div class="overlay">
              <!-- <span class="fa f"></span> -->
              <h2>Cuisine Share</h2>
              <p>a cuisine sharing platform</p>
            </div>
          <!-- </div> -->


        </div>
      </a>


      <a href="https://monstergame-gamma.vercel.app/" target="_blank" class="card item">
        <div class="card-content">
          <img class="card-img"  src="../assets/img/portfolio/monstergame.png" alt="monster game"/>
          <div class="overlay">
            <!-- <span class="fa f"></span> -->
            <h2>Monster Game</h2>
          <p>a mini monster game</p>
          </div>

        </div>
      </a>


      <a href="https://movie-series-overview.vercel.app/" target="_blank" class="card item">
        <div class="card-content">
          <img class="card-img"  src="../assets/img/portfolio/movie-series-overview.png" alt="movie overview"/>
          <div class="overlay">
            <!-- <span class="fa f"></span> -->
            <h2>Movie Series Overview</h2>
            <p>a quick movie or series search</p>
          </div>

        </div>
      </a>


      <a href="https://vue-id-card-maker-xbyu.vercel.app/" target="_blank" class="card item">
        <div class="card-content">
          <img class="card-img" src="../assets/img/portfolio/vue-id-card-maker.png" alt="ID Card"/>
          <div class="overlay">
            <!-- <span class="fa f"></span> -->
            <h2>ID Card</h2>
          <p>an id card generator</p>
          </div>

        </div>
      </a>





                    

  </div>

</section>
</template>
  

<style scoped>
.body {
  display: flex;
  gap: 25px;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  /* height: 100vh; */
  /* background-color: #f0f0f0; */
}

.card img {
  width: 30rem;
  height: 24rem;
}

.card {
  text-decoration: none;
  color: inherit; /* Inherit link color */
  width: 300px;
  border: 1px solid #ccc;
  border-radius: 8px;
  overflow: hidden;
  margin: 10px;
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-5px); /* Move card up slightly on hover */
}

.card-content {
  padding: 20px;
}

.card-content h2 {
  margin: 0;
}

.card-content p {
  margin-top: 10px;
  font-size: 0.9rem;
}

@media screen and (max-width: 768px) {
  /* For tablet view, display one card per row */
  .card {
    width: calc(100% - 20px);
    height:10rem;
  }
}

.card img {
  width: auto;
  /* width: calc(100% - 20px); */
  /* height: 24rem; */
}

.card:hover {
  transform: translateY(-5px);
}

.card-content {
  padding: 20px;
}

.card-content h2 {
  margin: 0;
}

.card-content p {
  margin-top: 10px;
  font-size: 0.9rem;
}
.overlay {
  margin-top: 15px;
    font-size: 25px;
    font-weight: 600;
    color: #fff;
}
</style>