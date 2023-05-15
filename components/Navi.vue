<template>
    <div>
      <nav class=" bg-black bg-opacity-70  text-gray-200 fixed top-0 left-0 right-0">
        <div class="flex items-center justify-between px-4">
          <div class="flex items-center">
            <!-- Icon on the left -->
            <div class="mr-2">
              <img src="@/assets/img/bean-removebg-preview.png" class="h-16 w-16" />
            </div>
            <span class="font-semibold">Beannsoft</span>
          </div>
          <div class="hidden md:flex md:items-center md:space-x-4">
            <ul class="flex space-x-4 text-base">
              <!-- Menu items on the right -->
              <li><a href="#" class="hover:text-gray-300">How we work</a></li>
              <li><a href="#" class="hover:text-gray-300">What we do</a></li>
              <li><a href="#" class="hover:text-gray-300">Pricing</a></li>
              <li><a href="#" class="hover:text-gray-300">Contact</a></li>
              <li><a href="#" class="hover:text-gray-300">Careers</a></li>
            </ul>
          </div>
          <!-- Menu toggle button (for mobile) -->
          <div class="flex items-center md:hidden bg-black bg-opacity-30">
            <button class="p-2" @click="menuOpen = !menuOpen">
              <Icon
                :name="menuOpen ? 'ic:outline-cancel' : 'ic:menu'"
                class="w-6 h-6 transition-transform duration-300 transform"
              />
            </button>
          </div>
        </div>
      </nav>
  
      <!-- Responsive menu (for mobile) -->
      <div class="md:hidden mt-10 pb-2 fixed w-full bg-black bg-opacity-70" v-show="menuOpen">
        <ul class="  text-gray-200 px-4 py-2 gap-y-5">
          <li><a href="#" class="block">How we work</a></li>
          <li><a href="#" class="block">What we do</a></li>
          <li><a href="#" class="block">Pricing</a></li>
          <li><a href="#" class="block">Contact</a></li>
          <li><a href="#" class="block">Careers</a></li>
        </ul>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        menuOpen: false,
      };
    },
  }
  </script>
  
  <style  scoped>
  /* Add any custom styles here */
  </style>
  