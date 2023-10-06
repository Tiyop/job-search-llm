<template>
  <v-layout>
      <v-app-bar title="Application bar"></v-app-bar>
      <v-main style="min-height: 300px;">
        <SearchPrompt />
      </v-main>
      
    </v-layout>

  
</template>

<script setup>
  import SearchPrompt from '@/components/SearchPrompt.vue'
</script>
