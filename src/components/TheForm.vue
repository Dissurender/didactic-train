<script setup lang="ts">
import { ref } from 'vue';
import BaseCard from './BaseCard.vue';
import DocumentationIcon from './icons/IconDocumentation.vue';

const test = ref('Test Text');
</script>

<template>
  <p>{{ test }}</p>

  <BaseCard>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Test Heading</template>

    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Non nesciunt, fugiat corporis
    consequatur ipsam voluptates suscipit molestiae eius voluptas quibusdam beatae ipsa nam
    perferendis? Dolorum, distinctio ullam. Aut, tempore iusto!
  </BaseCard>

  <BaseCard>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>

    Vue’s
    <a href="https://vuejs.org/" target="_blank" rel="noopener">official documentation</a>
    provides you with all information you need to get started.
  </BaseCard>
</template>
