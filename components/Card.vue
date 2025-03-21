<!-- src/components/Card.vue -->
<template>
    <div class="card">
        <h2>{{ title }}</h2>
        <p>{{ description }}</p>
    </div>
</template>

<script>
    export default {
        name: 'Card',
        props: {
            title: String,
            description: String
        }
    };
</script>

<style scoped>
    .card {
        background-color: #f9f9f9;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        margin: 20px;
        text-align: center;
    }
</style>  