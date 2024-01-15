<script setup>
import { Head } from '@inertiajs/vue3';

const props = defineProps({
    title: {
        type: String,
        default: 'App Title'
    }
});

const pageDescription = props.title + ' description';
</script>

<template>
    <Head>
        <title>{{ title }}</title>
        <meta name="description" :content="pageDescription">
    </Head>

    <div class="container">
        <slot/>
    </div>
</template>
