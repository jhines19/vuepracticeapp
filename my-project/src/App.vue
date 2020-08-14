<template>
  <div>
    <h1>{{ newMessage }}</h1>
    <heading></heading>
    <students v-bind:students="students"></students>
  </div>
</template>

<script>
import heading from './components/heading.vue'
import students from './components/students.vue'
export default {
  components:{
    'heading':heading,
    'students':students,
    },
  name: 'app',
  data () {
    return {
      newMessage:'Hello There!',

      students:[
        {name:'Jim', experience:'2'},
        {name:'Rob', experience:'3'},
        {name:'Tom', experience:'4'},
        {name:'Luke', experience:'5'},
        ]
    }
  }
}
</script>

<style scoped>
h1{
  color:green;
}
</style>
