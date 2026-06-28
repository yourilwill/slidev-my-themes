<template>
  <div class="slidev-layout cover h-full flex flex-col items-center justify-center text-center px-16">
    <slot />
  </div>
</template>

<style scoped>
.slidev-layout.cover {
  background: linear-gradient(135deg, #282a36 0%, #1e2029 100%);
}

.slidev-layout.cover :deep(h1) {
  font-size: 3rem;
  color: var(--dracula-purple);
  text-shadow: 0 0 24px rgba(189, 147, 249, 0.4);
  border-bottom: none;
  margin-bottom: 0.5rem;
}

.slidev-layout.cover :deep(p) {
  color: var(--dracula-comment);
  font-size: 1.2rem;
}
</style>
