<template>

  <div class="flex p-8 justify-center">
    <input type="text" class="rounded border-gray-200 w-full"
     placeholder="Search for Meals" />

    <div class="flex gap-1">
      <router-link  v-for="letter of letters.split("")">

      </router-link>
    </div>
  </div>
  
</template>



<script setup>
import store from '../store';
import { computed } from 'vue';

const meals = computed( () => store.state.meals);

const letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
</script>


