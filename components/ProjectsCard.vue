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
        <div class="h-60 border border black flex flex-col justify-around rounded-lg">
            <div>
                <p class="">{{ name.name }}</p>
                <button>View</button>
            </div>
        </div>
    </div>
</template>

<style scoped></style>