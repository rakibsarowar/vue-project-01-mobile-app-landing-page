<template>
    <div class="bg-gray-100">
      <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mx-auto max-w-2xl py-16 sm:py-24 lg:max-w-none lg:py-32">
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Meet our leadership</h2>
          <h2 class="mt-6 text-base leading-7 text-gray-600">We’re a dynamic group of individuals who are passionate about what <br> we do and dedicated to delivering the best results for our clients.</h2>
  
          <div class="mt-6 space-y-12 lg:grid lg:grid-cols-3 lg:gap-x-6 lg:space-y-0">
            <div v-for="callout in callouts" :key="callout.name" class="group relative">
              <div class="relative h-80 w-full overflow-hidden rounded-lg bg-white sm:aspect-h-1 sm:aspect-w-2 lg:aspect-h-1 lg:aspect-w-1 group-hover:opacity-75 sm:h-64">
                <img :src="callout.imageSrc" :alt="callout.imageAlt" class="h-full w-full object-cover object-center" />
              </div>
              <h3 class="mt-6 text-sm text-gray-500">
                <a :href="callout.href">
                  <span class="absolute inset-0" />
                  {{ callout.name }}
                </a>
              </h3>
              <p class="text-base font-semibold text-gray-900">{{ callout.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const callouts = [
    {
      name: 'Head Engineer ',
      description: 'Lary John',
      imageSrc: 'https://i.ibb.co/vzN4YTv/tream-1.jpg',
      imageAlt: 'Photo of Lary',
      href: '#',
    },
    {
      name: 'Head Designer',
      description: 'Rakib Sarowar',
      imageSrc: 'https://i.ibb.co/YdqJq0J/team-2-1.jpg',
      imageAlt: 'Photo of Rakib',
      href: '#',
    },
    {
      name: 'Project Manager',
      description: 'Ismail Haque',
      imageSrc: 'https://i.ibb.co/NTTJ5mb/team-2-2.jpg',
      imageAlt: 'Photo of Ismail',
      href: '#',
    },
  ]
  </script>
<style></style>
