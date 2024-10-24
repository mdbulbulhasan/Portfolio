<script setup>

import DropdownMenu from "@/components/SideMenu.vue";
import SideMenu from "@/components/SideMenu.vue";


const navItems = [
  {
    text: 'Home',
    route: '/',
    id:'#home',
  },
  {
    text: 'About',
    route: '/about',
    id:'#about',
  },
  {
    text: 'Services',
    route: '/services',
    id:'#services',
  },
  {
    text: 'Skills',
    route: '/skills',
    id:'#skills',
  },
  {
    text: 'Work',
    route: '/work',
    id:'#work',
  },
  {
    text: 'Contact',
    route: '/contact',
    id:'#contact',
  },
];
</script>
<template>
  <nav class="fixed top-0 left-0 w-full z-50 flex justify-evenly items-center border-2  font-semibold text-white p-5">
    <div class="flex lg:w-[20%] w-full lg:w- justify-between">
      <a href="" class="text-4xl">Portfo <span class="text-yellow-400">lio</span></a>
      <div>
        <SideMenu/>
      </div>

    </div>
      <ul class="flex justify-center items-center gap-10 lg:text-3xl text-xl">

        <li v-for="item in navItems" :key="item.text" class="lg:flex md:flex hidden lg:W-[80%] hover:text-yellow-400">
<!--          <router-link :to="item.route">{{ item.text}}</router-link>-->
          <a :href="item.id">{{ item.text }}</a>

        </li>

      </ul>

  </nav>
</template>