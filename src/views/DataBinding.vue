<template>
    <div>
        <!-- <label><input type="checkbox" value="서울" v-model="checked">서울</label>
        <label><input type="checkbox" value="부산" v-model="checked">부산</label>
        <label><input type="checkbox" value="제주" v-model="checked">제주</label>
        <br>
        <span>체크한 지역: {{checked}}</span> -->
        <!-- 체크박스 예제 -->

        <!-- <label><input type="radio" v-bind:value="radioValue1" v-model="picked">서울</label>
        <label><input type="radio" v-bind:value="radioValue2" v-model="picked2">부산</label>
        <label><input type="radio" v-bind:value="radioValue3" v-model="picked">제주</label>
        <br>
        <span>선택한지역 : {{picked}} {{picked2}}</span> -->
        <!-- 라디오버튼 예제 -->

        <!-- <img v-bin
        
        d:src="imgSrc"/> -->
        <!-- 이미지 예제 -->

        <!-- <input type="text" v-model="textValue" />
        <button type="button" v-bind:disabled="textValue==''">Click</button> -->
        <!-- 버튼 disabled예제 -->

        <!-- <div class="container" v-bind:class="{'active':isActive, 'text-red' : hasError}">Class Binding</div> -->
        <!-- 클래스 예제 -->

        <!-- <div class="container" v-bind:class="[activeClass, errorClass]">Class Binding</div> -->
        <!-- 배열을 사용한 클래스 예제 -->

        <!-- <div v-bind:style="styleObject">인라인 스타일 바인딩</div> -->
        <!-- 인라인 스타일 예제 -->

        <!-- <div v-bind:style="[baseStyle, addStyle]">인라인 스타일 바인딩</div> -->
        <!-- 배열을 이용한 인라인 스타일 예제 -->

        <!-- <table>
            <thead>
                <tr>
                    <th>제품명</th>
                    <th>가격</th>
                    <th>카테고리</th>
                    <th>배송료</th>
                </tr>
            </thead>
            <tbody>
                <tr :key="i" v-for="(product, i) in productList">
                    <td>{{product.product_name}}</td>
                    <td>{{product.price}}</td>
                    <td>{{product.category}}</td>
                    <td>{{product.delivery_price}}</td>
                </tr>
            </tbody>
        </table> -->
        <!-- 리스트 랜더링 예제 -->



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
            // return {
            //     picked : '',
            //     picked2 : '',
            //     radioValue1: `서울`,
            //     radioValue2: `부산`,
            //     radioValue3: `제주`
            // }
            // 라디오버튼 예제

           return {
            //  imgSrc : "https://icepipeled.com/wp-content/uploads/kboard_attached/1/202003/5e7c46800c59b6522402.png"
            // 이미지 예제

            // textValue:""
            // 버튼 disabled예제

            // isActive:true, 
            // hasError:false
            // 클래스 예제

            // activeClass : 'active',
            // errorClass : 'text-red'
            // 배열을 이용한 클래스 예제

            // styleObject:{
            //     color:'red',
            //     fontSize : '13px'
            // }
            // 인라인 스타일 예제
            
            // baseStyle : 'background-color:yellow; width:100%; height:200px;',
            // addStyle : 'color:red; font-weight:bold;'
            // 배열을 이용한 인라인 스타일 예제

            // productList : [
            //     {"product_name" : "기계식키보드", "price" : 25000, "category" : "노트북/태블릿", "delivery_price":5000},
            //     {"product_name" : "무선마우스", "price" : 12000, "category" : "노트북/태블릿", "delivery_price":5000},
            //     {"product_name" : "아이패드", "price" : 725000, "category" : "노트북/태블릿", "delivery_price":5000},
            //     {"product_name" : "태블릿거치대", "price" : 32000, "category" : "노트북/태블릿", "delivery_price":5000},
            //     {"product_name" : "무선충전기", "price" : 42000, "category" : "노트북/태블릿", "delivery_price":5000},
            // ]
            // 리스트 랜더링 예제

           }
        }
    }
</script>
<style scoped>
    /* container {
        width: 100%;
        height: 200px;
    }
    .active{
        background-color: yellow;
        font-weight: bold;
    }
    .text-red{
        color: red;
    } */
    /* 클래스 예제 */

    /* table{
        font-family: arial, sans-serif;
        border-collapse: collapse;
        width: 100%;
    }
    td,th{
        border: 1px solid #ddd;
        text-align: left;
        padding: 8px;
    } */
    /* 리스트 랜더링 예제 */

</style>