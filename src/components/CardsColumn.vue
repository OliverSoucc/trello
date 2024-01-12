<script setup>
import Card from './Card.vue';
import draggable from 'vuedraggable'
import {ref} from "vue";

const props = defineProps({
  columnTitle: String,
  cards: []
})

const myList = ref([...props.cards]
)
</script>

<template>
  <div class="flex-col">
  <h4 class="text-3xl font-semibold mb-4 text-gray-800">{{ columnTitle }}</h4>
  <div>
  <draggable v-model="myList" tag="ol" group="items">
    <template #item="{element}">
      <li class="mb-2">
        <Card :title="element.title" :description="element.description"/>
      </li>
    </template>
  </draggable>
  </div>
  </div>
</template>

<style scoped>

</style>