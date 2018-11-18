<template>
    <div>
        <div @click="isActive = true" class="notification is-warning">
            <h1 class="title is-size-6">{{ news.title }}</h1>
            <h2 class="subtitle is-size-7">{{ news.date }}</h2>
            <p class="is-size-7" v-html="news.content"></p>
        </div>
        <modal :isActive="isActive" @close="isActive = false">
            <p v-html="news.fullContent"></p>
        </modal>
    </div>
</template>

<script>
import Modal from './Modal.vue'
export default {
    name: 'NewsCard',
    props: ['news'],
    data () {
        return {
            isActive: false
        }
    },
    components: {
        Modal
    }
}
</script>

<style>

</style>
