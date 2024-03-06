<script setup lang="ts">
import { useI18n } from 'vue-i18n';
import Counter from '@/components/Counter.vue';

const { t, locale } = useI18n({
  inheritLocale: true,
  useScope: 'local',
});
</script>

<template>
  <div class="flex justify-center items-center">
    {{ $t('hello') }}
    <div class="i-mdi-home" />
  </div>
  <Counter />
</template>
