<template>
  <section class="bg-white overflow-hidden isolate relative" id="hero">
    <NavBar />
    <svg
      class="w-full h-full -z-10 inset-0 absolute stroke-[#e5e7eb]"
      style="
        mask-image: radial-gradient(100% 100% at top right, white, transparent);
      "
    >
      <defs>
        <pattern
          id="0787a7c5-978c-4f66-83c7-11c213f99cb7"
          width="200"
          height="200"
          x="50%"
          y="-1"
          patternUnits="userSpaceOnUse"
        >
          <path d="M.5 200V.5H200" fill="none"></path>
        </pattern>
      </defs>
      <rect
        width="100%"
        height="100%"
        stroke-width="0"
        fill="url(#0787a7c5-978c-4f66-83c7-11c213f99cb7)"
      ></rect>
    </svg>
    <div
      class="px-6 pt-40 lg:px-8 flex lg:flex-row justify-around max-w-7xl mx-auto relative"
    >
      <div
        class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80"
        aria-hidden="true"
      >
        <div
          class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-indigo-500 to-teal-500 opacity-30 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]"
          style="
            clip-path: polygon(
              74.1% 44.1%,
              100% 61.6%,
              97.5% 26.9%,
              85.5% 0.1%,
              80.7% 2%,
              72.5% 32.5%,
              60.2% 62.4%,
              52.4% 68.1%,
              47.5% 58.3%,
              45.2% 34.5%,
              27.5% 76.7%,
              0.1% 64.9%,
              17.9% 100%,
              27.6% 76.8%,
              76.1% 97.7%,
              74.1% 44.1%
            );
          "
        ></div>
      </div>
      <div class="max-w-[42rem] lg:max-w-[36rem] text-center lg:text-left">
        <h1
          class="text-gray-900 -space-x-0.5 font-bold mt-10 text-4xl sm:text-6xl"
        >
          Hey, I'm Mitch!
        </h1>
        <p class="text-gray-600 text-lg mt-6 leading-8">
          I'm a senior software engineer with a passion for building products
          that users love. I thrive on solving complex problems, especially
          where AI, performance, and great UX meet. I'm always pushing myself to
          learn more more about technology, UX, and AI.
        </p>
        <div class="mt-10 flex items-center justify-center gap-x-6">
          <a
            href="mailto:mitchell2077@gmail.com"
            class="rounded-md bg-teal-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-teal-600"
            >Contact me</a
          >
          <a
            href="#experience"
            class="text-sm font-semibold leading-6 text-gray-900"
            >Learn more <span aria-hidden="true">→</span></a
          >
        </div>
      </div>
      <div class="hidden lg:flex -mt-8 justify-center relative">
        <img
          src="https://cap-call.nyc3.cdn.digitaloceanspaces.com/public/CapCallHero.webp"
          alt=""
          class="w-64 h-[500px]"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import NavBar from '@/components/NavBar.vue';
</script>
