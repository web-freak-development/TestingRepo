<template>
    <div class="welcome">
        <h1>Welcome to Laravel with Inertia and Vue 3</h1>
        <p>Your application is ready!</p>
        <div class="links">
            <Link href="/about" class="btn">Learn More</Link>
        </div>
    </div>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<style scoped>
.welcome {
    text-align: center;
    padding: 2rem;
}

h1 {
    color: #333;
    margin-bottom: 1rem;
}

p {
    color: #666;
    margin-bottom: 2rem;
}

.links {
    margin-top: 2rem;
}

.btn {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    background-color: #007bff;
    color: white;
    border-radius: 0.25rem;
    text-decoration: none;
    transition: background-color 0.2s;
}

.btn:hover {
    background-color: #0056b3;
}
</style>