<template>
  <div class="max-w-3xl px-4 mx-auto sm:px-6 xl:max-w-5xl xl:px-0">
    <div class="pt-6 pb-8 space-y-2 md:space-y-5">
      <!-- <h1
        class="text-3xl font-extrabold leading-9 tracking-tight text-gray-900 dark:text-gray-100 sm:text-4xl sm:leading-10 md:text-6xl md:leading-14"
      >
        Projects
      </h1>
      <p class="text-lg leading-7 text-gray-500 dark:text-gray-400">
        Some of the projects I've build or been a part of.
      </p> -->
      <header class="pt-16 pb-9 sm:pb-16 sm:text-center">
        <h1 class="mb-4 text-8xl sm:text-4xl tracking-tight text-slate-800 font-extrabold dark:text-slate-200">
          Projects
        </h1>
        <p class="text-lg text-slate-700 dark:text-slate-400">
          Some of the projects I've build or been a part of.
        </p>
      </header>
    </div>
    <main class="relative mb-auto">
      <div class="">
        <div class="container py-12">
          <div class="flex flex-wrap -m-4">
            <project-card v-for="item in projectsData" :key="item.title" :title="item.title"
              :description="item.description" :href="item.href" :github="item.github" :tech1="item.tech1"
              :tech2="item.tech2" :tech3="item.tech3"></project-card>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
import projectsData from "../data/projects";
export default {
  data() {
    return {
      projectsData: projectsData,
    };
  },
  head: {
    title: "Ivan Alvarez | Projects",
    meta: [
      { charset: "utf-8" },
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        hid: "description",
        name: "description",
        content: "Some of Projects developed by or with Ivan",
      },
    ],
    link: [{ rel: "icon", type: "image/x-icon", href: "/favicon.ico" }],
  },
};
</script>
