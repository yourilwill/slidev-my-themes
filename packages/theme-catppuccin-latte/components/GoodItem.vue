<template>
  <span class="good-item">
    <mdi-emoticon-happy-outline class="good-icon" />
    <span class="good-label"><slot /></span>
  </span>
</template>

<style scoped>
.good-item {
  display: inline-flex;
  align-items: center;
}
.good-icon {
  font-size: 32pt;
  color: var(--ctp-green);
  background: rgba(64, 160, 43, 0.18);
  clip-path: circle(42%);
  margin-right: 0.3em;
  flex-shrink: 0;
}
.good-label {
  color: var(--ctp-green);
}
</style>
