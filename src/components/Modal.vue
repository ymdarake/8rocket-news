<template>
    <div class="modal" :class="{ 'is-active': isActive }">
        <div @click="close" class="modal-background"></div>
        <div class="modal-content">
            <div class="notification">
                <slot/>
            </div>
        </div>
        <button @click="close" class="modal-close is-large" aria-label="close"></button>
    </div>
</template>

<script>
export default {
    props: ['isActive'],
    methods: {
        close () {
            this.$emit('close')
        }
    }
}
</script>

<style>

</style>
