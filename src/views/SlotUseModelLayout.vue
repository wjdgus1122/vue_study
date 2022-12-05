<template>
    <model-layout>
        <template v-slot:header>
            <h1>팝업 타이틀</h1>
        </template>
        <template v-slot:default>
            <p>팝업 컨텐츠 1</p>
            <p>팝업 컨텐츠 2</p>
        </template>
        <template v-slot:footer>
            <button type="button">닫기</button>
        </template>
    </model-layout>
</template>
// v-slot대신에 단축어로 #을 사용할 수 있다.