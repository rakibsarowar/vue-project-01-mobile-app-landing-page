<template>
  <div>
    <div  class=" space-y-12 px-12 lg:grid lg:grid-cols-2 lg:gap-x-6 lg:space-y-0">
      <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
        <img id="about" :src="imageUrl" alt="">
      </div>
      <div  class="relative isolate px-6 pt-14 lg:px-8">
        <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
          <div class="text-center mx-auto w-4/6">
            <h1 class="text-3xl font-bold text-left tracking-tight text-gray-900 sm:text-4xl">About Us</h1>
            <p class="mt-6 text-base text-left leading-7 text-gray-600">{{ details }}</p>
            <div class="mt-10 flex items-left justify-left gap-x-6">
              <a href="#"
                class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">See
                Features</a>
            </div>
          </div>
        </div>
      </div>
    </div>
</div>
</template>
<script setup>
import { ref } from 'vue';
  const imageUrl = ref('https://i.ibb.co/cr8vb83/about.png');
  const details = ref(`Introducing our innovative web design mobile app! With a sleek and intuitive interface, it empowers users to effortlessly create stunning websites on the go. Packed with a wide range of customizable templates, advanced features, and seamless collaboration capabilities, it's the perfect tool for modern designers to bring their visions to life. Experience the future of web design today!`)
</script>
<style></style>