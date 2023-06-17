<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
import needWantSavingStats from '@/Components/NeedWantSavingStats.vue';



</script>

<template>
    <AppLayout title="Dashboard">
        <template #header>
            <h2 class="font-semibold text-xl text-base-content leading-tight">
                Dashboard
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <need-want-saving-stats :kyuuryou="7000"></need-want-saving-stats>

                <div class="bg-base-100 overflow-hidden shadow-xl sm:rounded-lg">

                </div>
            </div>
        </div>
    </AppLayout>
</template>
