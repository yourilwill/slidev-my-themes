<template>
  <div class="slidev-layout cover h-full flex flex-col items-center justify-center text-center px-16">
    <slot />
  </div>
</template>

<style scoped>
.slidev-layout.cover {
  background: linear-gradient(135deg, #1e1e2e 0%, #181825 100%);
}

.slidev-layout.cover :deep(h1) {
  font-size: 3rem;
  color: var(--ctp-mauve);
  text-shadow: 0 0 24px rgba(203, 166, 247, 0.4);
  border-bottom: none;
  margin-bottom: 0.5rem;
}

.slidev-layout.cover :deep(p) {
  color: var(--ctp-overlay0);
  font-size: 1.2rem;
}
</style>
