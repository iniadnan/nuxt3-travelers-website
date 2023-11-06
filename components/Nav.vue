<script setup>
const props = defineProps(['styles'])
</script>

<template>
    <!-- NAV -->
    <nav id="nav" class="w-full fixed z-50">
        <div class="container-travelers px-5 md:px-5 lg:px-0 z-20 relative">
            <div class="flex items-center md:gap-x-[48px] lg:gap-x-[70px] xl:gap-x-[80px] py-[14px]">
                <!-- HAMBURGER BUTTON SHOW IN MOBILE -->
                <div class="w-4/12 block md:hidden">
                    <button type="button" class="text-[#1E1E1E]">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                        </svg>
                    </button>
                </div>
                <!-- NAV LOGO -->
                <div class="w-4/12 md:w-auto">
                    <a href="/" class="font-heavitas text-base" :style="{ color: props.styles.color }">TRAVELERS</a>
                </div>
                <div class="hidden md:flex md:w-auto md:gap-x-[22px] lg:gap-x-[28px] xl:gap-x-[35px]">
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">Home</a>
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">About Us</a>
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">Destinations</a>
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">Travel Deals</a>
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">Blog</a>
                    <a href="/" class="font-medium text-base" :style="{ color: props.styles.color }">Services</a>
                </div>
                <!-- BOOK A TRAVEL -->
                <div class="w-4/12 md:w-auto flex justify-end ml-auto">
                    <!-- BUTTON BOOK TRAVEL -->
                    <a href="/"
                        class="inline-block py-[8px] px-[10px] md:py-[10px] md:px-[12px] lg:py-[13px] lg:px-[13px] font-bold text-sm md:text-base text-[#EDEDED] rounded-[10px] whitespace-nowrap"
                        style="background: linear-gradient(180deg, #0077ED -112.22%, #7BF9D3 196.67%);">Book <span
                            class="hidden md:inline-block">a travel</span>
                        <span class="inline-block md:hidden">Now</span>
                    </a>
                </div>
            </div>
        </div>
        <!-- SLIDE WHEN SCROLL -->
        <div class="absolute w-full h-full bg-white top-0 transform -translate-y-full transition duration-500" :style="{ transform: props.styles.transform }"></div>
    </nav>
</template>