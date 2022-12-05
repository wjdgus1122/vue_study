<template>
    <button type="button" @click="childFunc" ref="btn">자식 컴포넌트 데이터 변경</button>
    <!-- <h1>{{msg}}</h1> -->
</template>

<script>


export default {
    methods : {
        childFunc(){
            // console.log("부모 컴포넌트에서 직접 발생시킨 이벤트")
            this.msg = "변경된 메시지"
        },
        // callFromParent(){
        //     console.log("부모 컴포넌트에서 직접 호출한 함수");
        // }
    },
    data(){
        return {
            // msg:"자식 컴포넌트로부터 보내는 메시지"
            msg:"메시지"
        }
    },
    // mounted(){
    //     this.$emit('send-message', this.msg)
    // }
}
</script>