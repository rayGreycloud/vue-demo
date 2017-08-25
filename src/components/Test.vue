<template>
  <div class="test">
    <h1>{{title}}</h1>
    <p v-if="showName">{{user.firstName}}</p>
    <p v-else="showName">Friend</p>

  </div>
</template>

<script>
  export default {
    name: 'test',
    data() {
      return {
        title: "Hello",
        user: {
          firstName: 'John',
          lastName: 'Doe'
        },
        showName: false
      }
    }
  }
</script>

<style scoped></style>
