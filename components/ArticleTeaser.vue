<template>
  <a
    href="#"
    class="block px-6 py-4 border border-gray-500 rounded article-teaser"
  >
    <h2 class="pt-2 pb-4 text-2xl font-bold">
      {{ articleContent.title }}
    </h2>
    <p class="pb-6 leading-relaxed">
      {{ articleContent.intro }}
    </p>
    <p class="text-sm italic">
      {{ articleContent.author }}
    </p>
  </a>
</template>

<script>
export default {
  props: {
    articleContent: {
      type: Object,
      required: true
    }
  }
}
</script>

<style>
.article-teaser:hover {
  box-shadow: 0px 0px 15px 0px rgba(0,0,0,0.75);
}
</style>
