<template>
  <UBlogPosts>
    <UBlogPost v-for="(post, index) in posts" :key="index" v-bind="post" />
  </UBlogPosts>
</template>

<script setup lang="ts">
import type { BlogPostProps } from "@nuxt/ui";

const posts = ref<BlogPostProps[]>([
  {
    title: "Sample 1",
    description: "video view sample 1",
    image: "https://i.ytimg.com/vi/wh8OpTMgi7E/maxresdefault.jpg",
    date: "2024-11-25",
    to: "/works/1",
  },
]);
</script>
