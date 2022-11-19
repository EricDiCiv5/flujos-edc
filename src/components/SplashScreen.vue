<template>
    <div class="splashscreen">
        <img 
            src="@/assets/wave_flow.svg" 
            alt="Logo"
        />
        <h1><span>Flujos</span>EDC</h1>
    </div>
</template>

<script></script>

<style scoped>
.splashscreen {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
h1 {
  color: var(--brand-silver);
}
h1 span {
  color: var(--brand-gold);
}
</style>