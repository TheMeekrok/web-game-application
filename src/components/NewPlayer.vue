<template>
    <form @submit.prevent="onSubmit">
        <input type="text" v-model="name" />
        <button type="submit" class="add">Add</button>
    </form>
</template>

<script>
export default {
    data() {
        return {
            name: "",
        };
    },
    methods: {
        onSubmit() {
            if (this.name.trim()) {
                const newPlayer = {
                    id: Date.now(),
                    name: this.name,
                };

                this.$emit("new-player", newPlayer);
            }
        },
    },
};
</script>

<style>
form {
    display: flex;
}
.add {
    background: red;
}
</style>
