<script setup>

defineProps({
    name: {
        type: Object,
        required: true
    }
})

</script>
<template>
    <div>
        <div class="h-64 border border-blue-700 flex flex-col justify-around rounded-lg text-center">
            <div>
                <a :href="name.link" target="_blank">
                    <p class="hover:underline decoration-solid font-semibold mb-4">{{ name.name }}</p>
                    <span class="hover:text-blue-200">View</span>
                </a>
            </div>
        </div>
    </div>
</template>

<style scoped></style>