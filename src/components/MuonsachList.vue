<script>
export default {
    props: {
        muonsachs: { type: Array, default: [] },
        activeIndex: { type: Number, default: -1 },
    },
    emits: ["update:activeIndex"],
    methods: {
        updateActiveIndex(index) {
            this.$emit("update:activeIndex", index);
        }
    }
};
</script>
<template>
    <ul class="list-group">
        <li class="list-group-item" v-for="(muonsach, index) in muonsachs" :key="muonsach.madocgia"
            :class="{ active: index === activeIndex }" @click="updateActiveIndex(index)">
            {{ muonsach.madocgia }}
        </li>
    </ul>
</template>