<script setup>

const projectNames = [
    { name: 'Watches Online Store'},
    { name: 'Launch Mart' },
    { name: 'Dashboard-Iq' },
    { name: 'SokoMax' }
]
</script>
<template>
    <div class="grid grid-cols-2 gap-6">
       <ProjectsCard v-for="(project, index) in projectNames" :key="`id${index}`" :name="project" />
    </div>
</template>

<style scoped></style>