<template>
<div class="bg-white h-screen py-24 sm:py-32 flex justify-center items-center">
    <div class="mx-auto max-w-2xl rounded-3xl ring-1 ring-gray-200 py-36 max-w-7xl px-6 lg:px-8">
        <dl class="grid grid-cols-1 gap-x-20 gap-y-8 text-center lg:grid-cols-3">
            <div v-for="stat in stats" :key="stat.id" class="mx-auto flex max-w-xs flex-col gap-y-4">
                <dt class="text-base leading-7 text-gray-600">{{ stat.name }}</dt>
                <dd class="order-first text-3xl font-semibold tracking-tight text-blue-700 sm:text-5xl">{{ stat.value }}</dd>
            </div>
        </dl>
    </div>
</div>


</template>
  
<script setup>
const stats = [
    { id: 1, name: 'Happy Satisfied User', value: '0.5 millions' },
    { id: 2, name: 'Download', value: '$10 millions' },
    { id: 3, name: 'New users annually', value: '10,0000' },
]
</script>
<style></style>
