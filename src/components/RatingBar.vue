<template>
    <!-- Rating and Contact Container-->
    <div class="flex flex-wrap mt-2 items-center justify-between">
        <div class="flex items-center">
            <div
                v-for="i in 5"
                :key="i"
                :class="i <= apartments.rating ? 'bg-teal-400' : 'border-2 border-teal-400'"
                class="rounded-full w-3 h-3 mr-2"></div>
            <p class="ml-2 mr-2 font-semibold text-xs text-indigo-300 select-none">{{apartments.reviews}}
                reviews</p>
        </div>
    </div>
    <!-- Rating and Contact Container -->
</template>


<script>

export default {
    props : ['apartments']
}
</script>