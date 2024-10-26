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
        <a :href="name.link" target="_blank">
            <div class="  border border-blue-700 flex flex-col justify-around rounded-lg text-center p-6">
                <div class="hover:scale-105 ease-in-out duration-300">
                    <img class="rounded-lg" :src="name.image" />
                    <div>
                        <p class="hover:underline decoration-solid font-medium text-2xl">{{ name.name }}</p>
                        <span class="hover:text-blue-200">View</span>
                    </div>
                </div>
            </div>
        </a>
    </div>
</template>

<style scoped></style>