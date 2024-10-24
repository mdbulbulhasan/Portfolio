<script setup>

import DropdownMenu from "@/components/DropdownMenu.vue";
import {FontAwesomeIcon} from "@fortawesome/vue-fontawesome";

const navItems = [
  {
    text: 'Home',
    route: '/',
  },
  {
    text: 'About',
    route: '/about',
  },
  {
    text: 'Services',
    route: '/services',
  },
  {
    text: 'Skills',
    route: '/skills',
  },
  {
    text: 'Work',
    route: '/work',
  },
  {
    text: 'Contact',
    route: '/contact',
  },
];
</script>
<template>
  <nav class=" flex justify-evenly items-center font-semibold text-white p-5">
    <div class="flex lg:w-[20%] w-full border-2 lg:w- justify-between">
      <a href="" class="text-4xl">Portfo<span class="text-yellow-400">lio</span></a>
      <DropdownMenu/>
    </div>
      <ul class="flex justify-center items-center gap-10 text-xl">

        <li v-for="item in navItems" :key="item.text" class="lg:flex md:flex hidden lg:W-[80%]">
          <router-link :to="item.route">{{ item.text}}</router-link>
        </li>

      </ul>

  </nav>
</template>