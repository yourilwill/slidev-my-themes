<template>
  <div class="slidev-layout cover h-full flex flex-col items-center justify-center text-center px-16">
    <slot />
  </div>
</template>

<style scoped>
.slidev-layout.cover {
  background: linear-gradient(135deg, #eff1f5 0%, #e6e9ef 100%);
}

.slidev-layout.cover :deep(h1) {
  font-size: 3rem;
  color: var(--ctp-mauve);
  text-shadow: 0 0 24px rgba(136, 57, 239, 0.25);
  border-bottom: none;
  margin-bottom: 0.5rem;
}

.slidev-layout.cover :deep(p) {
  color: var(--ctp-overlay0);
  font-size: 1.2rem;
}
</style>
