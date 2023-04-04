<template>
  <div class="flexed">
    <h3>{{ comonentLocation() }} component from {{ origin }} app</h3>
  </div>
</template>

<script>
  export default {
    props: {
      origin: {
        type: String,
        default: 'local',
      }
    },
    methods: {
      comonentLocation() {
        return this.origin === 'local' ? ' Local' : 'Exposed'
      }
    }
  }
</script>

<style>
  h3 {
    color: rgb(100, 99, 99);
  }

  .img-size {
    height: 100px;
    width: 100px;
    margin-bottom: 15px;
  }

  .flexed {
    display: flex;
    align-items: center;
    border: 5px solid #2661A8;
    border-radius: 7px;
    flex-direction: column;
    width: 500px;
  }
</style>