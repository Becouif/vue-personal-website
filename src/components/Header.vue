<script setup>
import { ref } from 'vue';
import '../assets/css/header.css';

const isMenuOpen = ref(false);
const isDropdownOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value;
};
</script>

<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="brand-name">
          <a href="/" class="logo">
            <img class="img" src="../assets/img/logo/ABlogo.svg" alt="Logo">
          </a>
        </div>
        <div class="hamburger" @click="toggleMenu">
          <i class="fa fa-bars"></i>
        </div>
        <div class="navbar" :class="{ 'open': isMenuOpen }">
          <ul>
            <li><a href="#home" class="active">Home</a></li>
            <li class="dropdown-toggle" @click.stop="toggleDropdown">
              <a href="#about">About</a>
              <ul v-show="isDropdownOpen" class="dropdown-menu">
                <li><a href="#team">Our Team</a></li>
                <li><a href="#history">Our History</a></li>
              </ul>
            </li>
            <li><a href="#services">Services</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>