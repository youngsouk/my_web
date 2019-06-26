<template>
    <div class="container">
        <button class="btn btn-primary" @click="show = !show">
            Show
        </button>
        
        <transition name="fade">
            <div class="alert alert-info" v-if="show">
                Howdy! How cool is VueJS ?
            </div>
        </transition>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                show: false
            }
        }
    }
</script>
<style scoped>
    .fade-enter {
        opacity: 0;
    }

    .fade-enter-active {
        transition: opacity 1s;
    }


    .fade-leave-active {
        transition: opacity 1s;
        opacity: 0;
    }
</style>