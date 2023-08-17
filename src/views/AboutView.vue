<template>
    <div class="about">
        <h1>About</h1>
        <button @click="storeCounter.increaseCount" class="counter-btn">
            {{ storeCounter.count }}
        </button>
    </div>
</template>

<script setup>
    import { useCounterStore } from '../stores/counter';
    const storeCounter = useCounterStore()
</script>

<style>
    .counter-btn {
        font-size: 50px;
    }
</style>
