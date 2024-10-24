<script setup>
import { onMounted } from 'vue';
import Typed from 'typed.js';

onMounted(() => {
  const options = {
    strings: ["Web Developer", "Web Designer", "Freelancer"],
    typeSpeed: 100,
    backSpeed: 60,
    loop: true
  };

  // Initialize the Typed.js instance when the component is mounted
  const typed = new Typed('.typing', options);
});
</script>

<template>
  <div class="border-2 w-full lg:h-screen flex justify-start flex-col gap-[4rem] lg:pl-[15.5%] md:pl-[2%] pl-[6%]">
    <div class="flex flex-col lg:gap-6 gap-5 text-white font-semibold">
      <div class="lg:text-3xl text-xl">Hello, It's me</div>
      <div class="lg:text-5xl text-2xl w-[70%] lg:w-[50%]">Making your website attractive</div>
      <div class="lg:text-[5rem] lg:pt-10 text-2xl">And I'm a <span class="typing text-yellow-400"></span></div>
      <Button class="text-left pl-5 pr-5 mt-16 ease-in-out duration-300 ... lg:text-6xl text-2xl border border-yellow-500  bg-amber-400 w-fit p-2 rounded hover:-translate-y-2 hover:bg-background hover:text-yellow-400">Hire Me?</Button>
    </div>

    <div class="flex gap-8 lg:text-5xl lg:gap-[3rem] text-5xl cursor-pointer text-white">
      <a href="https://www.facebook.com/mdbulbulhasan09/" target="_blank" rel="noopener noreferrer"><font-awesome-icon :icon="['fab', 'facebook']" /></a>
      <a href="" target="_blank" rel="noopener noreferrer"><font-awesome-icon :icon="['fab', 'instagram']" /></a>
      <a href="https://github.com/mdbulbulhasan" target="_blank" rel="noopener noreferrer"><font-awesome-icon :icon="['fab', 'github']" /></a>
      <a href="https://www.linkedin.com/in/mdbulbulhasan/" target="_blank" rel="noopener noreferrer"><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
    </div>
  </div>

</template>