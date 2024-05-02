<template>
  <div class="bg-blue-400">
    <nav class="bg-white p-5 shadow md:flex md:items-center md:justify-between">
      <div class="flex items-center justify-between">
        <span class="text-3xl font-bold text-blue-500 cursor-pointer lg:mx-16">LOGO</span>
        <span class="text-3xl cursor-pointer mx-2 md:hidden block" onclick="menu()">
          <ion-icon name="menu-outline"></ion-icon>
        </span>
      </div>
      <ul class="md:flex md:items-center z-[-1] md:z-auto md:static absolute bg-white w-full left-0 md:w-auto md:py-0 py-4 md:pl-0 pl-7 md:opacity-100 opacity-0 top-[-400px] transition-all ease-in duration-500">
        <li class="mx-4 my-6 md:my-0">
          <nuxt-link to="/" class="mx-4 my-6 md:my-0">Home</nuxt-link>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <nuxt-link to="/service" class="mx-4 my-6 md:my-0">Service</nuxt-link>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <nuxt-link to="/tools" class="mx-4 my-6 md:my-0">Tools & Techonogi</nuxt-link>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <nuxt-link to="/work" class="mx-4 my-6 md:my-0">How We Work</nuxt-link>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <button class="px-5 py-2 bg-blue-500 text-white rounded-md">Get Started</button>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
function menu() {
  let list = document.querySelector("ul");
  list.classList.add("opacity-100");
}
</script>
