<template>
  <div class="p-8">
    <input type="text" v-model="keyword" @change="searchMeals" class="rounded border-2 border-gray-200 w-full"
      placeholder="Search for Meals" />

  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-5 p-8">
    <div v-for="meal in meals" :key="meal.idMeal" class="bg-white shadow">
      <img :src="meal.strMealThumb" alt="strMeal">
      <h3 class="px-3 py-2"> {{ meal.strMeal }} </h3>
      <div class="px-3 py-2">
        <a :href=" meal.strYoutube" target="_blank">Youtube</a>
        <router-link to="/"></router-link>
      </div>
    </div>
  </div>
    
</template>




<script setup>
import { computed } from '@vue/reactivity'
import { ref } from "vue"
import store from "../store"

const keyword = ref("")
const meals = computed(() => store.state.searchedMeals);

function searchMeals() {
  store.dispatch('searchMeals', keyword.value)
}

</script>
