<template>
  <div id="app">
    <my-header/>
    <router-view ></router-view>
    <table class="table">
    <thead>
    <task-rows>

    </task-rows>
  </thead>
 
    
  <input type="text" v-bind="task.todo">
  <input type="button" value="Create" @click="createTask">

  <tbody>
    <tr v-for="task in tasks" :key="task.id">
      <th scope="row">{{task.id}}</th>
      <td>{{task.name}}</td>
      <td>{{task.s_name}}</td>
      <td>{{task.todo}}</td>
    </tr>
  </tbody>
    </table>
  </div>
</template>

<script>
import MyHeader from './views/Components/MyHeader.vue'
import TaskRows from './views/Components/UI/TaskRows.vue'
export default {
  components: { MyHeader, TaskRows },
  data(){
    return{
      tasks:[
        {
          id:1,
          name:'qwe',
          s_name:'rrty',
          todo:'uio'
        },
        {
          id:2,
          name:'asd',
          s_name:'fgh',
          todo:'jkl'
        },
        {
          id:3,
          name:'zxc',
          s_name:'vbn',
          todo:'nm,.'
        },
      ],
      task:{
        id:4,
        name:'',
        s_name:'',
        todo:''
      }
    }
  },
  methods:{
    createTask(){
      this.tasks.push(this.task)
    }
  }
}
</script>

<style>

</style>