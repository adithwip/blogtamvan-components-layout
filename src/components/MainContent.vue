<template>
  <div class="col-md-9">
    <div class="list-group">
      <article-summary 
      v-for="(article, index) in articles" 
      :article="article" 
      :key="index"
      ></article-summary>
    </div>
  </div>
</template>

<script>
import ArticleSummary from '@/components/ArticleSummary'
export default {
  props: ['articles'],
  components: {
    ArticleSummary
  }
}
</script>

