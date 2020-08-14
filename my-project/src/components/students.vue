<template>
<div>
   <p v-for="student in students">{{student.name}} --> {{student.experience}}</p>
</div>

</template>

<script>
export default {
  props:['students'],
  data () {
    return {
    
    }
  }
}
</script>

<style>

</style>