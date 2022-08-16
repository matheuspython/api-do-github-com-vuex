<template>
  <header v-if="$store.state.user.login">Olaa {{$store.state.user.login}}</header>
  <header v-if="!$store.state.user.login">faça o login</header>
</template>

<script>
export default {};
</script>

<style scoped>
header {
  width: 100%;
  max-width: 100vw;
  height: 80px;
  background-color: #202024;
  color: #fff;
  box-shadow: #121214 0px 1rem 1.25rem;
  display: flex;
  align-items: center;
  justify-content: center;
  text-transform: uppercase;
}
</style>
