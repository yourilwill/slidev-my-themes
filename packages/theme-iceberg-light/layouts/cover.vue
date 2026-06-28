<template>
  <div class="slidev-layout cover h-full flex flex-col items-center justify-center text-center px-16">
    <slot />
  </div>
</template>

<style scoped>
.slidev-layout.cover {
  background: linear-gradient(135deg, #e8e9ec 0%, #dce0e8 100%);
}

.slidev-layout.cover :deep(h1) {
  font-size: 3rem;
  color: var(--ice-blue);
  text-shadow: 0 2px 8px rgba(45, 83, 158, 0.15);
  border-bottom: none;
  margin-bottom: 0.5rem;
}

.slidev-layout.cover :deep(p) {
  color: var(--ice-comment);
  font-size: 1.2rem;
}
</style>
