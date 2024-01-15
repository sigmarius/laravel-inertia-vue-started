<script setup>
import Layout from "../Shared/Layout.vue";

defineProps({
    title: {
        type: String
    }
});
</script>

<template>
    <Layout>
        <h1 class="text-2xl font-bold">Hello, {{ title }}!</h1>
    </Layout>
</template>
