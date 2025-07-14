<template>
  <header class="flex items-center gap-x-3">
    <!-- Avatar -->
    <section class="avatar avatar-online avatar-placeholder">
      <div class="bg-neutral text-neutral-content w-32 rounded-full">
        <span class="text-4xl">AJ</span>
      </div>
    </section>

    <section class="grow">
      <h1 class="sm:text-7xl text-4xl font-medium text-gray-800 dark:text-neutral-200">
        Alex John
      </h1>
      <p class="sm:text-4xl text-2xl text-gray-600 dark:text-neutral-400">
        Full Stack Developer, Content Creator
      </p>
    </section>
  </header>
  <!-- End Profile -->

  <!-- About -->
  <article class="mt-8">
    <Paragraph>
      I'm a remote full-stack developer and a content creator. currently,
      I work as a team leader of frontend-dev team.
    </Paragraph>
    <Paragraph class="mt-3">
      My expertise spans frontend
      development, backend development, SaaS integration and Cloud-Platform host.
    </Paragraph>
    <Paragraph class="mt-3">
      I help transform ideas into polished products by balancing rapid prototyping with clean, maintainable
      code—optimizing both velocity and quality.
    </Paragraph>
    <Paragraph class="mt-3">
      I'm keep making several free courses for beginners: <LinkPreview
        url="https://www.bilibili.com/video/BV1NNrvYQERH/" linkClass="hover:text-green-800 text-green-400" :width="400"
        :height="200">Vue Concise
      </LinkPreview>
      and
      <LinkPreview linkClass="hover:text-green-800 text-green-400" url="https://www.bilibili.com/video/BV1XS411c73U"
        :width="400" :height="200">
        Vue Advanced
      </LinkPreview>,
      <LinkPreview url="https://www.bilibili.com/video/BV1qK421x79b/" linkClass="hover:text-blue-800 text-blue-400"
        :width="400" :height="200">
        React Concise
      </LinkPreview> and
      <LinkPreview linkClass="hover:text-blue-800 text-blue-400" url="https://www.bilibili.com/video/BV1ow4m1r7fK"
        :width="400" :height="200">
        React Advanced
      </LinkPreview>,
      <LinkPreview url="https://www.bilibili.com/video/BV1GCoBY7ES3" linkClass="hover:text-green-800 text-[#589042]"
        :width="400" :height="200">
        NodeJS Concise
      </LinkPreview> etc.
    </Paragraph>

    <SocialLinks />
  </article>
</template>

<script setup lang="ts">
import LinkPreview from '../link-preview/LinkPreview.vue';
import Paragraph from './Paragraph.vue';
import SocialLinks from './SocialLinks.vue';

</script>