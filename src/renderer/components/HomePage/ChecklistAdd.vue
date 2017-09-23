<template>
  <div>
    <form @submit="formSubmitted">
      <div>
        <label for="name">
          List name
        </label>
        <input type="text" name="name" id="name">
      </div>
      <div>
        <input type="submit" value="Envoyer">
      </div>
    </form>
  </div>
</template>

<script>
  export default {
    methods: {
      formSubmitted(e) {
        console.log('form submitted', e);
        e.preventDefault();
      }
    }
  }
</script>

<style scoped>
  
</style>
