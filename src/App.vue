<template>
    <Suspense>
        <template #default>
            <SuperHome />
        </template>
        <template #fallback>
            <SplashScreen />
        </template>
    </Suspense>
</template>

<script>
import SplashScreen from "@/components/SplashScreen.vue";
import { defineAsyncComponent } from "vue";



export default {
    components: {
    SplashScreen,
    SuperHome: defineAsyncComponent(() => new Promise((resolve) => {
        setTimeout(() => {
            resolve(import("./components/SuperHome.vue"));
        }, 2000);
    })),
}
}
</script>

<style>
html, 
body, 
.app {
    min-height: 100vh;
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
}

* {
    --brand-gold: #bfba2d;
    --brand-silver: #999; 
}
</style>
