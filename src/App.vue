<script setup>
import Hero from '@/components/Hero.vue';
import Experience from '@/components/Experience.vue';
</script>

<template>
  <Hero />

  <section class="bg-white py-16 relative isolate" id="experience">
    <Experience />
    <div
      class="absolute inset-x-0 top-0 -z-10 transform-gpu overflow-hidden blur-3xl"
      aria-hidden="true"
    >
      <div
        class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-cyan-500 to-teal-500 opacity-30 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]"
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
    <div
      class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-35rem)]"
      aria-hidden="true"
    >
      <div
        class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-cyan-500 to-teal-500 opacity-30 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]"
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
  </section>
  <section class="bg-white pt-8 lg:pt-40" id="faq">
    <div
      class="px-10 max-w-[40rem] md:max-w-[80rem] flex flex-col md:flex-row justify-around mx-auto"
    >
      <div class="w-full pr-10">
        <h2 class="text-gray-900 leading-10 tracking-tight font-bold text-2xl">
          Frequently asked questions
        </h2>
        <p class="text-gray-600 text-base mt-4 leading-7">
          Can’t find the answer you’re looking for? Reach out to our
          <a href="#" class="text-teal-500 font-semibold whitespace-nowrap"
            >customer support</a
          >
          team.
        </p>
      </div>
      <div class="w-full mt-4 md:mt-0">
        <div>
          <span class="text-gray-900 leading-7 font-semibold text-base"
            >How do I start recording a call?
          </span>
          <p class="mt-2 text-gray-600 leading-7 text-base">
            Call to our Cap Call number, then click 'Add Call' to dial the
            person you wish to record with. Once they answer, click 'Merge Call'
            to start recording.
          </p>
        </div>
        <div class="mt-8">
          <span class="text-gray-900 leading-7 font-semibold text-base"
            >Is it legal to record phone calls?
          </span>
          <p class="mt-2 text-gray-600 leading-7 text-base">
            Laws regarding call recording vary by location. We advise checking
            your local laws to ensure compliance. In many regions, recording is
            legal with the consent of one or all parties involved.
          </p>
        </div>
        <div class="mt-8">
          <span class="text-gray-900 leading-7 font-semibold text-base"
            >Can the other person see that the call is being recorded?</span
          >
          <p class="mt-2 text-gray-600 leading-7 text-base">
            On iPhone only the person that started the three way call will now
            about the third call.
          </p>
        </div>
        <div class="mt-8">
          <span class="text-gray-900 leading-7 font-semibold text-base"
            >Will I be charged by my provider for the phone call?</span
          >
          <p class="mt-2 text-gray-600 leading-7 text-base">
            No, you will not be charged for calling the Cap Call phone number.
            We offer a toll-free number to ensure you will not be charged.
          </p>
        </div>
      </div>
    </div>
  </section>
  <div class="bg-white relative isolate">
    <div class="mx-auto max-w-7xl pt-24 sm:px-6 lg:px-8">
      <div class="mx-auto max-w-md text-center py-16 lg:py-32">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
          Boost your productivity.<br />Start using our app today.
        </h2>
        <p class="mt-6 text-lg leading-8 text-gray-600">
          Ready to transform the way you handle phone conversations? Download
          Cap Call today and experience the ultimate call recording solution.
          Try it now and never miss a detail again!
        </p>
        <div class="mt-10 flex items-center justify-center gap-x-6">
          <a
            href="/registration"
            class="rounded-md bg-teal-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-teal-600"
            >Get started</a
          >
          <a
            href="#features"
            class="text-sm font-semibold leading-6 text-gray-900"
            >Learn more <span aria-hidden="true">→</span></a
          >
        </div>
      </div>
    </div>
    <div
      class="absolute inset-x-0 top-10 -z-10 transform-gpu overflow-hidden blur-3xl flex justify-center"
      aria-hidden="true"
    >
      <div
        class="relative aspect-[1108/632] bg-gradient-to-tr from-indigo-500 to-teal-500 opacity-30 w-[69.25rem]"
        style="
          clip-path: polygon(
            73.6% 51.7%,
            91.7% 11.8%,
            100% 46.4%,
            97.4% 82.2%,
            92.5% 84.9%,
            75.7% 64%,
            55.3% 47.5%,
            46.5% 49.4%,
            45% 62.9%,
            50.3% 87.2%,
            21.3% 64.1%,
            0.1% 100%,
            5.4% 51.1%,
            21.4% 63.9%,
            58.9% 0.2%,
            73.6% 51.7%
          );
        "
      ></div>
    </div>
  </div>
  <footer class="bg-white pb-8 lg:px-8">
    <div
      class="max-w-[80rem] mx-auto border-t border-gray-200 pt-8 flex flew-row justify-between items-center text-xs"
    >
      <p class="text-gray-500 leading-5">
        © 2020 Cap Call, Inc. All rights reserved.
      </p>
      <div
        class="flex items-center justify-center cursor-pointer"
        @click="$router.push('/eula')"
      >
        <div class="underline text-gray-600">EULA</div>
      </div>
      <div
        class="flex items-center justify-center cursor-pointer"
        @click="$router.push('/terms-and-conditions')"
      >
        <div class="underline text-gray-600">Terms and Conditions</div>
      </div>
      <div
        class="flex items-center justify-center cursor-pointer"
        @click="$router.push('/privacy')"
      >
        <div class="underline text-gray-600">Privacy Policy</div>
      </div>
    </div>
  </footer>
</template>

<style scoped></style>
