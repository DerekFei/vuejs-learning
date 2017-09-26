<template>
  <div>
    <p> Server Status: {{status}} </p>
    <br>
    <button @click = "changeStatus"> Change Status </button>
  </div>
</template>

<script>
  export default{
    data: function(){
      return {
        status: 'Critical'
      }
    },
    methods: {
      changeStatus(){
        this.status = 'normal';
      }
    }
  }
</script>