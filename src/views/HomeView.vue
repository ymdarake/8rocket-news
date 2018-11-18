<template>
    <section class="section has-background-light">
      <div class="container">
        <div class="columns is-multiline">
          <div v-for="n in news" :key="n.title" class="column is-one-third">
              <news-card :news="n"/>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
import NewsCard from '../components/NewsCard.vue'
import { news } from '../api/news.js'

export default {
    data () {
        return {
            news
        }
    },
    components: {
        NewsCard
    }
}
</script>

<style>

</style>
