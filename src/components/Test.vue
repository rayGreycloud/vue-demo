<template>
  <div class="test">
    <input type="text" v-model="title"><br />
    <h1>{{title}}</h1>
    <p v-if="showName">{{user.firstName}}</p>
    <p v-else="showName">Friend</p>
    <ul>
      <li v-for="item in items">{{item.title}}</li>
    </ul>

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
        showName: true,
        items: [
          {title: 'Item One'},
          {title: 'Item Two'},
          {title: 'Item Three'}
        ]
      }
    }
  }
</script>

<style scoped></style>
