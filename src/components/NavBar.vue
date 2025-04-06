<template>
  <header class="absolute inset-x-0 top-0 z-50">
    <nav
      class="flex items-center justify-between p-6 lg:px-8"
      aria-label="Global"
    >
      <div class="flex lg:flex-1">
        <a href="#" class="-m-1.5 p-1.5">
          <div class="inline-flex items-center">
            <span class="text-sm font-semibold leading-6 text-gray-900 ml-2"
              >Mitch Moore</span
            >
          </div>
        </a>
      </div>
      <div class="hidden lg:flex lg:gap-x-12">
        <a
          v-for="item in navigation"
          :key="item.name"
          :href="item.href"
          class="text-sm font-semibold leading-6 text-gray-900"
          >{{ item.name }}</a
        >
      </div>
      <div class="flex lg:flex-1 lg:justify-end">
        <a href="/resume" class="text-sm font-semibold leading-6 text-gray-900"
          >Resume <span aria-hidden="true">&rarr;</span></a
        >
      </div>
    </nav>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const navigation = ref([
  { name: 'Experience', href: '#experience' },
  { name: 'Education', href: '#education' },
  { name: 'Projects', href: '#projects' },
  { name: 'Contact', href: 'mailto:mitchell2077@gmail.com' },
]);
</script>
