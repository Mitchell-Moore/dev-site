<template>
  <div class="mx-auto max-w-6xl px-6 lg:px-8">
    <div class="mx-auto max-w-2xl text-center">
      <!-- <h2 class="text-base font-semibold leading-7 text-teal-500">
        Work Experience
      </h2> -->
      <p
        class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl"
      >
        My Work Experience
      </p>
      <p class="mt-6 text-lg leading-8 text-gray-600 text-left">
        I have 4 years of experience working as a software engineer. I've worked
        at startups and large companies alike. I've had the opportunity to start
        as the first full time engineer and see the company grow to over 15
        employees! I try to learn something new every day and apply it to my
        work.
      </p>
    </div>
    <div class="space-y-12 mt-24">
      <div
        v-for="(job, index) in workExperience"
        :key="index"
        class="border-l-2 border-gray-200 pl-6 pb-2"
      >
        <!-- <div
          class="flex flex-col md:flex-row md:justify-between md:items-start mb-4"
        >
          <div>
            <h3 class="text-2xl font-bold text-gray-800">
              {{ job.company }}
            </h3>
            <p class="text-gray-600 mt-1">
              {{ job.role }}
            </p>
            <p class="text-gray-600 mt-2">
              {{ job.description }}
            </p>
          </div>
          <div
            class="mt-2 md:mt-0 md:ml-4 text-gray-500 font-medium md:text-right whitespace-nowrap"
          >
            {{ job.period }}
          </div>
        </div> -->
        <div>
          <div class="flex flex-col md:flex-row mb-4 justify-between">
            <div class="flex flex-col">
              <h3 class="text-2xl font-bold text-gray-800">
                {{ job.company }}
              </h3>
              <p class="text-gray-600 mt-1">
                {{ job.role }}
              </p>
            </div>
            <div
              class="mt-2 md:mt-0 md:ml-4 text-gray-500 font-medium md:text-right whitespace-nowrap"
            >
              {{ job.period }}
            </div>
          </div>
          <p class="text-gray-600 mt-2">
            {{ job.description }}
          </p>
        </div>

        <div class="mt-6" v-if="job.projects">
          <h4 class="text-lg font-semibold text-gray-700 mb-3">Key Projects</h4>
          <ul class="space-y-6">
            <li
              v-for="(project, projectIndex) in job.projects"
              :key="projectIndex"
              class="p-4 rounded-lg"
            >
              <h5 class="font-semibold text-gray-800">
                {{ project.name }}
              </h5>
              <p class="text-gray-600 mt-2">
                {{ project.description }}
              </p>
              <div class="mt-3 flex flex-wrap gap-2">
                <span
                  v-for="(tech, techIndex) in project.technologies"
                  :key="techIndex"
                  class="px-2 py-1 bg-gray-200 text-gray-700 text-xs rounded-full"
                >
                  {{ tech }}
                </span>
              </div>
            </li>
          </ul>
        </div>
        <div class="mt-1" v-if="job.points">
          <ul class="list-disc list-inside">
            <li
              v-for="(point, pointIndex) in job.points"
              :key="pointIndex"
              class="p-1 rounded-lg text-gray-600"
            >
              {{ point }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

// Sample data - replace with your actual work experience
const workExperience = ref([
  {
    company: 'Virtual Hallway',
    role: 'Senior Software Engineer',
    period: 'Jun 2021 - Present',
    description:
      'At Virtual Hallway, I help build the platform from zero to over 10,000+ consults. We enable real-time consults between physicians, specialists, and pharmacists resolving 84% of cases without in-person referrals and significantly easing the load on the healthcare system. As part of a fast-moving, clinician-led team, I’ve worked on features like AI-Powered medical scribe, automated medical billing, scalable medical education platform, and scalable infrastructure that supports thousands of consults across Canada. ',
    projects: [
      {
        name: 'Medical Scribe',
        description:
          'I developed a scalable AI medical scribe system that transcribes and summarizes medical consultations in real time, significantly reducing the administrative load on physicians and enhancing patient care efficiency. My key contributions included building core features such as outgoing call handling, consultation summarization, a correction layer to boost transcription accuracy, and a feedback loop to support continuous improvement. At launch, the product received a 4.8/5 user satisfaction rating, with physicians highlighting its ease of use and time-saving benefits. I also designed a dynamic deployment algorithm for our machine learning resources, which eliminated idle time, saved approximately $300 per day in cloud costs, and improved system responsiveness during peak hours. One of the most impactful improvements was a correction layer powered by Retrieval-Augmented Generation (RAG) and advanced prompt engineering, which increased medication name recognition accuracy from 62% to 98% — a critical enhancement for clinical reliability.',
        technologies: [
          'Vue.js',
          'Laravel',
          'Azure Machine Learning Studio',
          'Llama 3',
          'Swift',
          'Python',
        ],
      },
      {
        name: 'Patient-Oriented Evidence that Matters (POEMs)',
        description:
          'I led the implementation of Patient-Oriented Evidence that Matters (POEMs), a daily bite-sized medical education platform for physicians across Canada. Focused on UX and scalability, ensuring a seamless transition as our company became the new provider for all Canadian physicians. Designed a UI with list virtualization, infinite scroll, and scroll retention for an optimal scrolling and discoverability. Optimized performance and scalability with Redis caching, pagination, and local frontend caching, reducing load times and enhancing responsiveness. Resulted in thousands of doctors signing up and tens of thousands of medical education credits claimed per month.',
        technologies: ['Vue.js', 'Laravel', 'Redis', 'Klaviyo'],
      },
      {
        name: 'Medical Pathway Recommendations',
        description:
          'As part of a research initiative with a national research council, I contributed to building a system that helps physicians explore recommended medical pathways based on natural language queries. Doctors could input questions (e.g., "What are treatment options for early-stage diabetes?"), and the system would return relevant clinical pathways based on semantic similarity. This project combined NLP, vector search, and real-world healthcare data to support more informed clinical decisions. It was a great opportunity to apply machine learning in a meaningful, real-world context while working with a multidisciplinary team.',
        technologies: [
          'Python',
          'PostgreSQL',
          'FastAPI',
          'Docker',
          'Llama 3',
          'Hugging Face',
        ],
      },
      // {
      //   name: 'Doctor-IME (Independent Medical Examination)',
      //   description:
      //     'As part of a research initiative with a national research council, I contributed to building a system that helps physicians explore recommended medical pathways based on natural language queries. Doctors could input questions (e.g., "What are treatment options for early-stage diabetes?"), and the system would return relevant clinical pathways based on semantic similarity. This project combined NLP, vector search, and real-world healthcare data to support more informed clinical decisions. It was a great opportunity to apply machine learning in a meaningful, real-world context while working with a multidisciplinary team.',
      //   technologies: [
      //     'Vue.js',
      //     'Laravel',
      //     'Redis',
      //     'Docker',
      //     'Python',
      //     'PostgreSQL',
      //     'FastAPI',
      //     'LLMs',
      //   ],
      // },
    ],
  },
  {
    company: 'Lockheed Martin',
    role: 'Technical Co-op: Software – Internal Research and Development',
    period: 'Jan 2021 - Jun 2021',
    description:
      'At Lockheed Martin, I worked remotely on a small, fast-moving Agile team embedded within a much larger defense software ecosystem. Our team focused on maintaining and improving a mission-critical, high-throughput system built in Java. Much of our work involved navigating and optimizing a large legacy codebase, where performance, reliability, and security were paramount due to the nature of the system’s use in defense operations. During my time there, I:',
    points: [
      'Improved VM CPU by 17%, through using a code analyzer in a high throughput system.',
      'Implemented a dead reckoning algorithm to predict the movement of vessels and munitions.',
      'Acquired NATO security clearance.',
    ],
  },
]);
</script>
