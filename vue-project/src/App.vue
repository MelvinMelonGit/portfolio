<script setup>
import Navbar from "./components/Navbar.vue";
import Hero from "./components/Hero.vue";
import Contact from "./components/Contact.vue";
</script>

<template>
  <div class="text-neutral-50 font-custom">
    <div class="bg-stone-950 px-16">
      <Navbar />
      <main>
        <header>
          <Hero />
        </header>
      </main>
    </div>
    <Contact />
  </div>
</template>
