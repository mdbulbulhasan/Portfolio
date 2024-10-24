<script setup>
import NavBar from "@/components/NavBar.vue";
import HomeContent from "@/components/HomeContent.vue";
</script>

<template>
  <!--  Home Section Start-->
  <section id="home">
    <div class="bg-custom-bg border-4 border-yellow-500 bg-cover lg:h-screen md:h-full h-screen">
      <div>
        <NavBar/>
      </div>
      <div class="lg:pt-[8%] md:pt-[15%] pt-[35%]">
        <HomeContent/>
      </div>
    </div>
  </section>
  <!--  Home Section End-->

  <!--  About Section Start-->
  <section id="about">
    <div class="bg-stone-900 h-screen">

    </div>
  </section>
  <!--  About Section Start-->

  <!--  Service Section Start-->

  <!--  Service Section End-->
</template>/