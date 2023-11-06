<script setup lang="ts">
import { ref, reactive, computed, watch } from 'vue';
import BaseCard from './BaseCard.vue';
import DocumentationIcon from './icons/IconDocumentation.vue';

const data = reactive([]);

const firstName = ref('');
const lastName = ref('');
const city = ref('');

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

  <input v-model="firstName" placeholder="First Name" />
  <input v-model="lastName" placeholder="Last Name" />
  <input v-model="city" placeholder="City" />
</template>
