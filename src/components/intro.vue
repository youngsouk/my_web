<template>
    <div>
        <transition name="fade">
            <div id="logo_center" v-if="fresh">
                <img  id = "logo" alt="TRUST_LOGO" src="./../assets/TRUST_logo.png">
            </div>
        </transition>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                fresh: true
            }
        },
        mounted() {
            setTimeout(() => {
                this.fresh = !this.fresh
            }, 500);
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
    #logo_center{
        text-align : center;
    }
    #logo{
        margin: 0 auto;
        position: fixed;
        z-index : 1;
        top : 25%;
        left : 25%;
        width : 48%;

    }
</style>