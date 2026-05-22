<template>
    <MainLayout>
        <div class="bg-white rounded-lg shadow-md p-8">
            <h1 class="text-4xl font-bold mb-4 text-gray-900">
                About
            </h1>
            <p class="text-gray-600 text-lg mb-6">
                {{ about }}
            </p>
            <div class="bg-blue-50 border-l-4 border-blue-600 p-4 mb-6">
                <h2 class="text-xl font-bold text-blue-900 mb-2">
                    Tech Stack
                </h2>
                <ul class="text-blue-800 space-y-2">
                    <li>✅ Laravel 13 - Modern PHP Framework</li>
                    <li>✅ Inertia JS - SPA approach with Laravel</li>
                    <li>✅ Vue 3 - Progressive JavaScript Framework</li>
                    <li>✅ Vite - Next Generation Frontend Tooling</li>
                    <li>✅ Tailwind CSS - Utility-first CSS Framework</li>
                </ul>
            </div>
            <Link href="/" class="inline-block bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
                Back Home
            </Link>
        </div>
    </MainLayout>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
import MainLayout from '@/Layouts/MainLayout.vue';

defineProps({
    about: String,
});
</script>