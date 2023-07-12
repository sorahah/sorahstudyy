<template>
    <div>
        안녕 {{username}}들아
        {{ numberOfVisit }} 번째 방문
    </div>
   
</template>
<script>
export default {
    name: "testTxt",
    props:{
        username: String,
        numberOfVisit: Number,
    }
}
</script>