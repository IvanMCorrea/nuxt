<script setup>
const { data } = useLazyFetch("/api/posts");
</script>

<template>
  <div v-for="(post, index) in data.data" class="mx-5 my-5">
    <article class="p-3 bg-gray-300 dark:bg-gray-700 rounded-xl">
      <h3>{{ index + 1 }} - {{ post?.title }}:</h3>
      <p>
        {{ post?.body }}
      </p>
    </article>
  </div>
</template>
