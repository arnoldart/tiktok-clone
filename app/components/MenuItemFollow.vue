<template>
    <div class="flex items-center hover:bg-gray-100 rounded-md w-full py-1.5 px-2">
        <img 
            class="rounded-full lg:mx-0 mx-auto"
            width="35"
            src="https://yt3.ggpht.com/yti/ANjgQV9VfxfC1OlAGXhpMXvPhiPKNxarjplJ9PRUdCMGp_Ma5H4=s88-c-k-c0x00ffffff-no-rj" 
            alt=""
        >
        <div class="lg:pl-2.5 lg:block hidden">
            <div class="flex items-center">
                <div class="font-bold text-[14px]">
                    User Name
                </div>
                <div class="ml-1 rounded-full bg-[#58D5EC] h-[14px] relative">
                    <Icon class="relative -top-[3.3px] bg-white" name="teenyicons:tick-small-solid" size="15" />
                </div>
            </div>
            <div class="font-light text-[12px] text-gray-600">
                User Name
            </div>
        </div>
    </div>
</template>

<script setup>
    defineProps(['user'])
</script>