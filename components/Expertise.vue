<template>
  <div class="mt-8">
    <div class="mt-2">
      <h2 class="mb-2 text-xl text-gray-700 font-bold dark:text-blue-200 capitalize">
        Frontend
      </h2>

      <ul class="flex flex-wrap gap-4 items-center">
        <!-- <li class="flex items-center">
          <Html class="h-10 w-10 rounded-sm drop-shadow-sm"> </Html>
        </li>
        <li class="flex items-center">
          <Css class="h-10 w-10 rounded-sm drop-shadow-sm"></Css>
        </li> -->
        <li class="flex items-center">
          <Javascript class="h-10 w-10"></Javascript>
        </li>
        <li class="flex items-center">
          <Typescript class="h-10 w-10"></Typescript>
        </li>
        <li class="flex items-center">
          <Vuejs class="h-10 w-10"></Vuejs>
        </li>
        <li class="flex items-center">
          <Nuxt class="h-10 w-10"></Nuxt>
        </li>
        <li class="flex items-center">
          <TailwindCss class="h-10 w-10"></TailwindCss>
        </li>
        <li class="flex items-center">
          <Ionic class="h-10 w-10"></Ionic>
        </li>
        <li class="flex items-center">
          <Angular class="h-10 w-10"></Angular>
        </li>
        <!-- <li class="flex items-center">
          <Bootstrap class="h-10 w-10"></Bootstrap>
        </li> -->
      </ul>
    </div>
    <div class="mt-4">
      <h2 class="mb-2 text-xl text-gray-700 font-bold dark:text-blue-200 capitalize">
        Backend
      </h2>
      <ul class="mb-6 flex flex-wrap gap-4">
        <li class="flex items-center">
          <Laravel class="h-10 w-10"></Laravel>
        </li>
        <li class="flex items-center">
          <Node class="h-10 w-10"></Node>
        </li>
        <li class="flex items-center">
          <Python class="h-10 w-10"></Python>
        </li>
      </ul>
    </div>
    <div class="mt-4">
      <h2 class="mb-2 text-xl text-gray-700 font-bold dark:text-blue-200 capitalize">
        Tools
      </h2>
      <ul class="mb-6 flex flex-wrap gap-4">
        <li class="flex items-center">
          <Docker class="h-10 w-10"></Docker>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import Javascript from "../assets/devicon/javascript.svg?inline";
import Typescript from "../assets/devicon/typescript-plain.svg?inline";
import Html from "../assets/devicon/html.svg?inline";
import Css from "../assets/devicon/css.svg?inline";
import Vuejs from "../assets/devicon/vuejs.svg?inline";
import TailwindCss from "../assets/devicon/tailwindcss.svg?inline";
import Nuxt from "../assets/devicon/nuxt.svg?inline";
import Bootstrap from "../assets/devicon/bootstrap.svg?inline";
import Laravel from "../assets/devicon/laravel-new.svg?inline";
import Node from "../assets/devicon/node.svg?inline";
import Docker from "../assets/devicon/docker-original.svg?inline";
import Angular from "../assets/devicon/angularjs-original.svg?inline";
import Ionic from "../assets/devicon/ionic-original.svg?inline";
import Python from "../assets/devicon/python-plain.svg?inline";
export default {
  components: {
    Javascript,
    Typescript,
    Html,
    Css,
    Bootstrap,
    Vuejs,
    TailwindCss,
    Nuxt,
    Laravel,
    Docker,
    Angular,
    Ionic,
    Node,
    Python,
  },
};
</script>
