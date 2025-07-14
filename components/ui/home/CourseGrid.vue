<template>
  <div class="flex items-center justify-center my-2 w-full">
    <AnimateGrid :cards>
      <template #logo="{ logo }">
        <img class="logo mx-auto h-10 w-auto" :src="logo" />
      </template>
    </AnimateGrid>
  </div>
</template>
<script lang="ts" setup>
import AnimateGrid from "../animate-grid/AnimateGrid.vue";
import vue from "~/public/imgs/vue.svg";
import react from "~/public/imgs/react.svg";
import nodejs from "~/public/imgs/nodejs.svg";
import git from "~/public/imgs/git.svg";
import gitee from "~/public/imgs/gitee.svg";
import supabase from "~/public/imgs/supabase.svg";
import shadcn from "~/public/imgs/shadcn.svg";
import materialui from "~/public/imgs/materialui.svg";
import daisyui from "~/public/imgs/daisyui.svg";
import shoelace from "~/public/imgs/shoelace.svg";
import docker from "~/public/imgs/docker.svg";
import more from "~/public/imgs/more.svg";

const cards = [{
  logo: vue,
  link: "https://www.bilibili.com/video/BV1NNrvYQERH/",
  desc: "Vue",
},
{
  logo: react,
  link: "https://www.bilibili.com/video/BV1qK421x79b/",
  desc: "React",
},
{
  logo: nodejs,
  link: "https://www.bilibili.com/video/BV1GCoBY7ES3",
  desc: "NodeJS",
},
{
  logo: git,
  link: "https://www.bilibili.com/video/BV1Hkr7YYEh8/",
  desc: "Git",
},
{
  logo: gitee,
  link: "https://www.bilibili.com/video/BV1bRN2enEtV/",
  desc: "Gitee",
},
{
  logo: supabase,
  link: "https://www.bilibili.com/video/BV1LJ4m1K7SX/",
  desc: "Supabase",
},
{
  logo: shadcn,
  link: "https://www.bilibili.com/video/BV1ye411v7Q2/",
  desc: "Shadcn",
},
{
  logo: materialui,
  link: "https://www.bilibili.com/video/BV1Ci421Q72o/",
  desc: "Material UI",
},
{
  logo: daisyui,
  link: "https://www.bilibili.com/video/BV1fY9JY8E5x/",
  desc: "daisyUI",
},
{
  logo: shoelace,
  link: "https://www.bilibili.com/video/BV1xw411N7hM/",
  desc: "Shoelace",
},
{
  logo: docker,
  link: "https://www.bilibili.com/video/BV1vxcweoEJS/",
  desc: "Docker",
},
{
  logo: more,
  link: "/courses",
  desc: "Explore more courses",
}
]
</script>