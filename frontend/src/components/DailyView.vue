<template>
  <ul>
    <li class="timeslot" v-for="(item, index) in timeslots" :key="index">
      {{ item.time }} <base-todo-card title="test"></base-todo-card>
    </li>
  </ul>
</template>

<script>
import BaseTodoCard from './base-components/BaseTodoCard.vue'

export default ({
    components: { BaseTodoCard },
    data() {
        return {
            timeslots: [
                { time: '8:00' },
                {time: '9:00' }, 
                { time: '10:00' }
            ]
        }
    },
})
</script>

<style scoped>
.timeslot{
    display: flex;
    align-content: center;
    margin-right: 10px;

}
</style>
