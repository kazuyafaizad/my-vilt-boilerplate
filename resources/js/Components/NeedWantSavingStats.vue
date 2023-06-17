<script setup>

defineProps({
    kyuuryou: {
        type: Number,
        default: 0,
    },
});


</script>

<template>
    <div class="stats shadow bg-neutral w-full">

        <div class="stat">
            <div class="stat-figure">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                    class="inline-block w-8 h-8 stroke-current">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z">
                    </path>
                </svg>
            </div>
            <div class="stat-title">Needs</div>
            <div class="stat-value" title="house/car/food/internet">{{ kyuuryou * 0.5 }}</div>
            <div class="stat-desc">50%</div>
        </div>

        <div class="stat">
            <div class="stat-figure ">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                    class="inline-block w-8 h-8 stroke-current">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z">
                    </path>
                </svg>
            </div>
            <div class="stat-title">Wants</div>
            <div class="stat-value " title="netflix/">{{ kyuuryou * 0.3 }}</div>
            <div class="stat-desc">30%</div>
        </div>

        <div class="stat">
            <div class="stat-figure ">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                    class="inline-block w-8 h-8 stroke-current">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z">
                    </path>
                </svg>
            </div>
            <div class="stat-title">Savings/Lends</div>
            <div class="stat-value " title="creditcard/asb">{{ kyuuryou * 0.2 }}</div>
            <div class="stat-desc">20%</div>
        </div>

    </div>
</template>
