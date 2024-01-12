<script >
import {defineComponent} from "vue";
import Column from "@/components/CardsColumn.vue";

export default defineComponent({
  components: {Column}

})
</script>

<template>
<div class="flex gap-20 justify-center pt-20 px-20">
  <Column :columnTitle="'Backlog:'" :cards="[
      {title:'Weekend Getaway Planning', description: 'Plan an exciting weekend getaway with friends and family'},
      {title:'Culinary Adventure', description: 'Explore new recipes and create a delicious homemade dinner'},
      {title:'Language Learning Journey', description: 'Learn a new language and impress others with your linguistic skills.'},
      {title:'Explore Local Hiking Trails', description: 'Embark on an adventurous journey through scenic trails, discover hidden waterfalls'},
      {title:'Create a DIY Home Garden', description: 'Transform your backyard into a lush oasis with colorful flowers, aromatic herbs.'},
      {title:'Learn to Play a Musical Instrument', description: 'Master the art of playing a musical instrument'},
      {title:'Weekly Productivity Challenge', description: 'Boost your productivity with a weekly challenge. Tackle tasks, set goals'},
      {title:'Create a DIY Home Garden', description: 'Transform your backyard into a lush oasis with colorful flowers, aromatic herbs.'},
      {title:'Learn to Play a Musical Instrument', description: 'Master the art of playing a musical instrument'},
      {title:'Weekly Productivity Challenge', description: 'Boost your productivity with a weekly challenge. Tackle tasks, set goals'},
    ]"/>
  <Column :columnTitle="'In Progress:'" :cards="[
      {title:'Garden Design Project', description: 'Design a beautiful garden layout with vibrant flowers and plants'},
      {title:'Virtual Landmark Tou', description: 'Embark on a virtual tour of historical landmarks around the world.'},
    ]"/>
  <Column :columnTitle="'Done:'" :cards="[
      {title:'New Workout Routine', description: 'Try a new workout routine to stay active and healthy.'},
    ]"/>
</div>
</template>

<style scoped>

</style>