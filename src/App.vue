<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import FloatLabel from 'primevue/floatlabel';
import Checkbox from 'primevue/checkbox';
import CheckboxGroup from 'primevue/checkboxgroup';

import InputText from 'primevue/inputtext';


import { ref } from "vue";

const pizza = ref();



const value = ref(null);
</script>


<template>
  <div class="card flex flex-wrap justify-center gap-4">
      <div class="flex items-center gap-2">
          <Checkbox v-model="pizza" inputId="ingredient1" name="pizza" value="Cheese" />
          <label for="ingredient1"> Cheese </label>
      </div>
      <div class="flex items-center gap-2">
          <Checkbox v-model="pizza" inputId="ingredient2" name="pizza" value="Mushroom" />
          <label for="ingredient2"> Mushroom </label>
      </div>
      <div class="flex items-center gap-2">
          <Checkbox v-model="pizza" inputId="ingredient3" name="pizza" value="Pepper" />
          <label for="ingredient3"> Pepper </label>
      </div>
      <div class="flex items-center gap-2">
          <Checkbox v-model="pizza" inputId="ingredient4" name="pizza" value="Onion" />
          <label for="ingredient4"> Onion </label>
      </div>


      <div class="card flex justify-center">
        <FloatLabel>
            <InputText id="username" v-model="value" variant="filled" />
            <label for="username">Username</label>
        </FloatLabel>
    </div>
  </div>
</template>


