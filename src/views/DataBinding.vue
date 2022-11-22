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

        <!-- <div>
            <h1 v-if="type=='A'">A</h1>
            <h1 v-else-if="type=='B'">B</h1>
            <h1 v-else>C</h1>
            <h1 v-show="bShow == 'A'">bShow</h1>
        </div> -->
        <!-- 랜더링 문법(v-if, v-show) v-if는 toggle형식. 조건이 true일때 html이 삭제가 되거 생성됨
        그러나 v-show는 처음 랜더링 될때 html이 생기고 css로 display가 바뀌는 형식. 형식이 자주 바뀌면 v-show를 쓰는게 좋고, 자주 바뀌지 않는다면 v-if를 쓰는게 좋다.
         -->

        <!-- <button type="button" @click="increaseCounter">Add 1</button>
        <p>The counter is : {{counter}}</p> -->
        <!-- <button type="button" @click="setCount(7)">Add 1</button>
        <p>The counter is : {{counter}}</p> -->
        <!-- <button type="button" @click="one(), two()">Click</button> -->
        <!-- Click 이벤트 -->

        <!-- <select v-model="selectedValue" @change="changeSelect">
            <option value="서울">서울</option>
            <option value="부산">부산</option>
            <option value="제주">제주</option>
        </select> -->
        <!-- change이벤트 -->

        <!-- <input @keyup.enter="submit" /> -->
        <!-- key이벤트 ==> 어떤 키가 입력되었는지 감지 할 수 있는 이벤트 위에 예시같은 경우는 enter키의 입력을 감지할 수 있다. -->
        <!-- <input @keyup.alt.enter = "clear"/> -->
        <!-- Alt + Enter키 감지 -->
        <!-- <div @click.ctrl="doSomething">Do something</div> -->
        <!-- Ctrl + Click -->
        <!-- Key 이벤트 -->

        <!-- <h1>{{firstName + ' '+ lastName}}</h1> -->
        <!-- <h1>{{getFullName()}}</h1> -->
        <!-- <h1>Full Name : {{fullName}}</h1> -->
        <!-- computed : 데이터베이스에서 데이터를 불러올 경우 처음 값을 화면에서 보여주고, 데이터값이 바뀔때마다 computed함수 실행 . 첫번째 예제와 두번째 예제는 화면에 보여줘야 하는만큼
        함수를 호출하거나 연산해야함. computed는 데이터가 바뀔때 한번만 실행됨-->

        <h1>Full Name : {{fullName}}</h1>
        <button type="button" @click="changeName">변경</button>
        <!-- watch : 처음랜더링 할때 초기값을 받았을때는 값에 변화가 없다고 인식되어 값이 표출되지 않는다. 데이터베이스에서 데이터가 바뀌어야 화면에 함수가 실행되면서 표출됨. -->


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

            // type : 'B',
            // bShow : 'A'
            // 랜더링 예제(v-if, v-show)

            // counter : 0
            // click이벤트예제

            // selectedValue : '서울'
            // change이벤트

            firstName : 'Seungwon',
            lastName : 'Go',
            fullName : ''
           }
        },
        // computed : {
        //     fullName(){
        //         return this.firstName + ' ' + this.lastName;
        //     }
        // },

        watch : {
            firstName(){
                this.fullName = this.firstName + ' ' + this.lastName;
            },
            lastName(){
                this.fullName = this.firstName + ' ' + this.lastName;
            }
        },

        methods : {
            // increaseCounter(){
            //     this.counter = this.counter + 1;
            // }
            // setCount(counter){
            //     this.counter = counter;
            // }
            // one(){
            //     alert('One')
            // },
            // two(){
            //     alert('Two')
            // }
            // click이벤트 예제

            // changeSelect(){
            //     alert(this.selectedValue)
            // }
            // change이벤트

            // getFullName(){
            //     return this.firstName + ' ' + this.lastName;
            // }

            changeName(){
                this.firstName = 'Eunsol';
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