<script setup>
import { computed } from 'vue'
import { useStore } from 'vuex';
// import Login from "./components/LoginComp.vue";


const store = useStore()
const user = computed(() => store.state.user)


</script>

<template>
    <div class="w-screen">
        <!-- <pre>{{ user }}</pre> -->
        <!-- <Login /> -->
        <router-view></router-view>
    </div>
</template>

<style scoped>
.logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
}

.logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
    filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
