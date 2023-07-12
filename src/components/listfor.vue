<template>
    <li v-for="item in arr" v-bind:key="item"> {{ item }} </li>

</template>
<script>
export default {
    name: "lsitfor",
    props:{
        item: Array,
    },
    data() {
        return {
            arr: this.item, // item을 arr로 변경
        };
    },
    
}</script>