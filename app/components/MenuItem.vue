<template>
    <div class="w-full flex items-center hover:bg-gray-100 p-2.5 rounded-md">
        <div class="flex items-center lg:mx-0 mx-auto">
            <Icon :name="icon" :color="colorString" :size="sizeString" />
            <span
                :class="`text-[${colorString}]`"
                class="lg:block hidden pl-[9px] mt-05 font-semibold text-[17px]"
            >
                {{ iconString }}
            </span>
        </div>
    </div>
</template>

<script setup>

const props = defineProps([
    'iconString',
    'colorString',
    'sizeString'
]);

const { iconString, colorString, sizeString } = toRefs(props);

let icon = '';

if(iconString.value === 'For You') {
    icon = 'mdi:home';
} else if (iconString.value === 'Following') {
    icon = 'ci:group';
} else if (iconString.value === 'LIVE') {
    icon = 'ri:live-line';
}

</script>