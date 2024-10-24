<script setup>
const buttons = [
    { name: 'About', route: '/about' },
    { name: 'Projects', route: '/projects' },
    { name: 'Resume', route: '/Resume' },
]
</script>

<template>
    <div>
        <div class="flex justify-around text-gray-500 font-semibold">
            <nav v-for="(nav, index) in buttons" :key="`id-${index}`">
                <NuxtLink :to="nav.route">{{ nav.name }}</NuxtLink>
            </nav>
        </div>
    </div>
</template>

<style scoped>

</style>