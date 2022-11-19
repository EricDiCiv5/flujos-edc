<template>
    <header>
        <img
            @click="reload"
            src="@/assets/wave_flow.svg" 
            alt="Logo" 
        />
        <h1><span>Flujos</span>EDC</h1>
        <span></span>
    </header>
</template>

<script>
export default {
    methods: {
        reload () {
            location.reload();
        }
    }
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100vw;
}
img,
span {
  width: 48px;
}
h1 {
  font-size: 1.4rem;
  color: var(--brand-silver);
}
h1 span {
  color: var(--brand-gold);
}
</style>