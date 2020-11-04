<template>
  <div class="container">
    <h1>Welcome to Z-Vue</h1>
    <img class="logo" src='https://note.ss.purevivi.chat/Fnn562fSUBw4HdUH7GOH8sWD0GnH'>
     <a href='#/page1'>page1</a>
  </div>
</template>

<script>
export default {
  name: 'Hello Home',
  props: {
    msg: String
  }
}
</script>

<style lang="scss">
.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
}

.logo {
    width: 100px;
    height: 100px;
    border-radius: 50%;
}

h1{
  color: $blue;
}

</style>
