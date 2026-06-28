<template>
  <span class="bad-item">
    <mdi-emoticon-sad-outline class="bad-icon" />
    <span class="bad-label"><slot /></span>
  </span>
</template>

<style scoped>
.bad-item {
  display: inline-flex;
  align-items: center;
}
.bad-icon {
  font-size: 32pt;
  color: #880e4f;
  background: #fce4ec;
  clip-path: circle(42%);
  margin-right: 0.3em;
  flex-shrink: 0;
}
.bad-label {
  color: #880e4f;
}
</style>
