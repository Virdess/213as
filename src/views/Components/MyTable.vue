<template>
  <div>
    <table class="table">
  <thead>
    <task-rows>

    </task-rows>
  </thead>
  <tbody>
    <task-rows>
      <task-id></task-id>
      <task-name></task-name>
      <task-sname></task-sname>
      <task-todo></task-todo>
    </task-rows>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td colspan="2">Larry the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>

  </div>
</template>

<style>

</style>


<script>
import TaskRows from './UI/TaskRows.vue'
export default {
  components: { TaskRows },
  props:{
    tasks:{
      type: Object,
      required: true,
    }
  },

}
</script>