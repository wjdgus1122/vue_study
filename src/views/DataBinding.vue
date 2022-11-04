<template>
    <div>
        <!-- <label><input type="checkbox" value="서울" v-model="checked">서울</label>
        <label><input type="checkbox" value="부산" v-model="checked">부산</label>
        <label><input type="checkbox" value="제주" v-model="checked">제주</label>
        <br>
        <span>체크한 지역: {{checked}}</span> -->
        <label><input type="radio" v-bind:value="radioValue1" v-model="picked">서울</label>
        <label><input type="radio" v-bind:value="radioValue2" v-model="picked2">부산</label>
        <label><input type="radio" v-bind:value="radioValue3" v-model="picked">제주</label>
        <br>
        <span>선택한지역 : {{picked}} {{picked2}}</span>
    </div>
</template>

<script>
    export default {
        // data() {
        //     return {
        //         checked : []
        //     };
        // }
        data(){
            return {
                picked : '',
                picked2 : '',
                radioValue1: `서울`,
                radioValue2: `부산`,
                radioValue3: `제주`
            }
        }
    }
</script>
