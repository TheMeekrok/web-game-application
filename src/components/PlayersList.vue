<template>
    <ul>
        <NewPlayer
            @new-player="addPlayer"
        />
        <PlayerListItem 
            v-for="player in players" 
            v-bind:player="player" 
        />
    </ul>
</template>

<script>
import PlayerListItem from "./PlayerListItem.vue";
import NewPlayer from "./NewPlayer.vue";
export default {
    data() {
        return {
            players: [{ id: 1, name: "dsfdsf" }],
        };
    },
    methods: {
        addPlayer(newPlayer) {
            this.players.push(newPlayer);
        }
    },
    components: {
    PlayerListItem,
    NewPlayer
},
};
</script>

<style scoped>
ul {
    list-style: none;
    margin: 0;
    padding: 0;
    width: 25%;
    height: 25%;
}
</style>
