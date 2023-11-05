<template>
  <div class="card">
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.card {
  border: 1px solid var(--color-border);
  border-radius: 7px;
  margin-top: 2rem;
}

.details {
  margin: 1rem;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;

  color: var(--color-heading);
}
</style>
