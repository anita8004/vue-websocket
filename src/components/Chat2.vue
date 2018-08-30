<template>
  <div class="websocket-chat">
    <div class="container">
      <form id="getName">
        <input type="text" name="name">
        <button type="submit">SEND</button>
      </form>
      <div id="chatRoom">
        <div class="users">
          <h3 class="listName">USERS</h3>
          <ul>
            <!-- <li> {{user}} </li> -->
          </ul>
        </div>
        <div class="chatBox">
          <div class="chatBoard"></div>
          <form class="chatForm">
            <input type="text">
            <button type="submit">↩</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Chat',
  data () {
    return {
      users: [],
      messages: {},
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
