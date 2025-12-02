<template>
    <div 
        id="SideNavMain"
        :class="route.fullPath === '/' ? 'lg:w-[310px]' : 'lg-w-[220px]'"
        class="fixed z-20 bg-white pt-[70px] h-full lg:border-r-0 border-r border-gray-300 w-[75px] overflow-auto"
    >
        <div class="lg:w-full w-[7t5px] mx-auto">
            <NuxtLink to="/">
                <MenuItem iconString="For You" colorString="#F02C56" sizeString="30" />
            </NuxtLink>
            <MenuItem iconString="Following" colorString="#000000" sizeString="27" />
            <MenuItem iconString="LIVE" colorString="#000000" sizeString="27" />
        </div>

        <div class="border-gray-300 border-b lg:ml-2 mt-2"></div>

        <div class="lg:block hidden text-xs text-gray-600 font-semibold pt-4 pb-2 px-2">
            Suggested Account
        </div>

        <div class="lg:hidden block pt-3"></div>

        <div class="cursor-pointer">
            <MenuItemFollow />
        </div>
    </div>
</template>

<script setup>

const route = useRoute();

</script>