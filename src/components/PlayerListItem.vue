<template>
    <li>
        <span>
            <strong>{{ player.id }}</strong>
            {{ player.name }}
        </span>
    </li>
</template>

<script>
export default {
    props: {
        player: {
            type: Object,
            required: true,
        },
    },
};
</script>

<style scoped>
li {
    border: 1px solid #ccc;
    display: flex;
    justify-content: space-between;
    padding: 0.5rem 2rem;
    margin-bottom: 1rem;
}
</style>
