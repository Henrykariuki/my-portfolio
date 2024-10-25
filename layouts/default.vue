<script setup>

</script>

<template>
    <div class="flex flex-col md:flex-row md:gap-2 md:p-6 h-screen">
        <div>
            <LeftPanel />
        </div>
        <div class="grow overflow-auto ">
            <div class="p-4">
                <MyHeader />
                <div>
                    <slot />
                </div>
            </div>
            <Footer />
        </div>
    </div>
</template>

<style scoped>
/* The entire scrollbar */
::-webkit-scrollbar {
    width: 12px;
    /* width of the scrollbar */
    height: 12px;
    /* height for horizontal scrollbar */
}

/* The track (background of the scrollbar) */
::-webkit-scrollbar-track {
    background: transparent;
    /* color of the track */
    border-radius: 10px;
    /* rounded edges for the track */
}

/* The handle (scroll indicator) */
::-webkit-scrollbar-thumb {
    background: #e47c059a;
    /* color of the scrollbar handle */
    border-radius: 10px;
    /* rounded edges for the handle */
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
    background: #ef8205cf;
    /* darker color when hovering */
}
</style>