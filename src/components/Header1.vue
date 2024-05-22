<script setup>
// import '../assets/css/header1.css';
import { onMounted } from 'vue';

onMounted(() => {
  const navbar = document.querySelector(".navbar");
  const links = navbar.querySelectorAll("a");
  const hamBurger = document.querySelector(".hamburger");

  links.forEach((element) => {
    element.addEventListener("click", function () {
      links.forEach(link => link.classList.remove("active"));
      this.classList.add("active");
      navbar.classList.remove("show");
    });
  });

  hamBurger.addEventListener("click", () => {
    navbar.classList.toggle("show");
  });
});
</script>

<template>
   <header>
     <div class="container">
       <div class="row">
         <div class="brand-name">
           <a href="/" class="logo">
             <img class="img" src="../assets/img/logo/ABlogo.svg" alt="">
           </a>
         </div>
         <div class="hamburger">
           <i class="fa fa-bars"></i>

         <div class="navbar">
           <ul>
             <li><a href="#home" class="active">Home</a></li>
             <li><a href="#about">About</a></li>
             <li><a href="#services">Services</a></li>
             <li><a href="#portfolio">Portfolio</a></li>
             <!-- <li><a href="#blog">Blog</a></li> -->
             <li><a href="#contact">Contact</a></li>
           </ul>
         </div>
         <!-- end of hamburger  -->
      </div>
       </div>
     </div>
   </header>
 </template>



<style scoped>

header {
  position: absolute;
  padding: 0px 15px;
  left: 0px;
  right: 0px;
  border-bottom: 1px solid #423940;
  z-index: 11;
}

.fixed {
  background-color: rgb(236, 241, 250);
  position: fixed;
  border-color: #eee;
  animation: fixHeader 1s ease;
  z-index: 11;
}

@keyframes fixHeader {
  0% {
    transform: translateY(-100%);
  }

  100% {
    transform: translateY(0%);
  }
}

.container {
  max-width: 1140px;
  margin: auto;
}

header .row {
  justify-content: space-between;
  align-items: center;
}

.brand-name a {
  /* margin-right: 50px; */
  font-size: 22px;
  font-weight: 500;
  color: rgb(236, 241, 250);
  position: relative;
  font-family: 'Lobster', cursive;
}

.fixed .brand-name a {
  color: #000;
}

.hamburger .fa {
  font-size: 20px;
  background-color: rgb(236, 241, 250);
  color: #01143e;
  display: none;
  height: 30px;
  width: 35px;
  border-radius: 2px;
  line-height: 30px;
  text-align: center;
  cursor: pointer;
  border: 1px solid #eee;
}

.navbar ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.navbar ul li {
  display: inline;
  margin-left: 35px;
}

.navbar ul li a {
  font-size: 15px;
  line-height: 72px;
  color: rgb(236, 241, 250);
  font-weight: 600;
  /* display: block; */
  position: relative;
}

.fixed .navbar ul li a {
  color: #000;
}

.navbar ul li a::before {
  content: "";
  height: 2px;
  background-color: rgb(236, 241, 250);
  width: 0%;
  position: absolute;
  right: 0px;
  bottom: -27px;
  cursor: pointer;
  transition: all 0.5s ease;
}

.fixed .navbar ul li a::before {
  background-color: #5f88e0;
}

.navbar ul li a:hover::before {
  width: 100%;
  left: 0px;
}

.navbar ul li a.active::before {
  width: 100%;
  left: 0;
}

a.logo img.img{
  /* margin-right: 10rem; */
  /* padding-left: 50px; */
width: 140px;
height: 100px;
margin-bottom: -20px;
/* padding: -100px; */
/* margin: -100px; */
}



/* Responsive styles */
@media screen and (max-width: 800px) {
  header {
    background-color: #0a0504;

  }
  .navbar {
    display: none;
    flex-direction: column;
    width: 100%;

    
  }

  .navbar.show {
    display: grid;
    color:#000;
    border: none;
    width: 10px;
    margin-left: 23.5rem;
    background: inherit;
  }

  .navbar ul {
    flex-direction: row;
    
  }

  .navbar ul li {
    margin-left: 0;
  }

  .hamburger .fa {
    display: block;
  }
}

</style>


