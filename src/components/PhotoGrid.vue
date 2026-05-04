<script setup lang="ts"></script>

<template>
  <section id="gallery">
    <h2><slot name="header"></slot></h2>
    <div class="gallery-container">
      <slot name="body"></slot>
    </div>
  </section>
</template>

<style scoped>
#gallery {
  padding: var(--padding-large);
  height: fit-content;
  min-width: 90vh;
  align-content: center;
  text-align: center;
  min-height: 100vh;
}

h2 {
  font-size: 3rem;
  padding: calc(var(--padding-large) * 2);
  color: var(--complement-colour);
}

.gallery-container {
  display: flex;
  justify-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  text-align: center;
  min-height: calc(100vw / 3.45);
}
</style>
