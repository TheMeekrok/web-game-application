<template>
    <div>
      <PlayersList/>
    </div>
</template>

<script>
import PlayersList from './components/PlayersList.vue'
export default {
    name: 'App',
    components: {
        PlayersList,
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
