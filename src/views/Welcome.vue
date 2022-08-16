<template>
    <main>
        <div class="container">
            <div class="box">
                <img :src="$store.state.user.avatar_url" :alt="$store.state.user.name + ' image'">
                <h1>{{$store.state.user.name}}</h1>
                <p>{{$store.state.user.login}}</p>
            </div>
        </div>

        <button @click="returnar">retornar</button>
    </main>
</template>

<script>
export default {
    name: 'WelcomeVue',
    methods: {
        returnar(){
             this.$router.push('/')
        }
    },
}
</script>

<style scoped>
main {
    width: 100%;
}
.container{
    display: flex;
    justify-content: center;
    align-items: center;
    height: calc(100vh - 80px);
}

.box{
    background: #2f3136;
    padding: 15px;
    text-align: center;
}
button{
    position: absolute;
    bottom: 15px;
    left: 50%;
    transform: translate(-50px,0 );
    width: 100px;
    max-width: 400px;
}

 button {
  background-color: transparent;
  border: 1px solid #8257e5;
  color: #fff;
  border-radius: 12px;
  height: 45px;
  transition: 0.4s;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  gap: 5px;
  font-size: 15px;
}

button:hover,
button:focus {
  background-color: #8257e5;
}

</style>