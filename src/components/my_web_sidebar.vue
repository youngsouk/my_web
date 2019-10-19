<template>
    <div>
        <button class="myButton" @click="onClickMenu">ㅡ
        </button>

        <transition name="menu-slide">
            <div id="menu-content" v-show="show">
                <br id = "text">
                <br id = "text">
                <p id="text" v-for = "menu in menus" v-bind:key="menu">
                    {{menu}}
                </p>
            </div>
        </transition>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                show: false,
                menus : ["메인", "포너블", "상남자", "웹", "TEST", "심심", "테트리스", "리버스", "c2w2m2", "스터디", "죽창", "죽창"]
            }
        },
        methods: {
            onClickMenu() {
                this.show = !this.show
            }
        }
    }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Noto+Sans+KR&display=swap');
    ul {
        text-align: left;
    }

    li {
        list-style-type: none;
        left: 0px;
    }

    #text {
        position: relative;
        vertical-align: middle;
        margin : 0 0 0 0;
        font-family: 'Noto Sans KR', sans-serif;
        font-size: 27px;
        color : #ffffff;
        margin-bottom: 6%;
    }

    #menu-content {
        position: fixed;
        z-index: 1;
        margin: 0 0 0 0;
        width: 30%;
        height: 100%;
        top: 0%;
        left: -2%;
        background-color: #000000; 
        text-align: center;
        vertical-align: middle;
        overflow: hidden;
        z-index: 0;
    }

    .menu-slide-enter-active {
        transition: all .5s ease;
    }

    .menu-slide-leave-active {
        transition: all .5s cubic-bezier(1.0, 0.5, 0.8, 1.0);
    }

    .menu-slide-enter,
    .menu-slide-leave-to {
        transform: translateX(-80px);
        opacity: 0;
    }

    .myButton {
        -moz-box-shadow: inset 0px 1px 0px 0px #ffffff;
        -webkit-box-shadow: inset 0px 1px 0px 0px #ffffff;
        box-shadow: inset 0px 1px 0px 0px #ffffff;
        background: -webkit-gradient(linear, left top, left bottom, color-stop(0.05, #ffffff), color-stop(1, #f6f6f6));
        background: -moz-linear-gradient(top, #ffffff 5%, #f6f6f6 100%);
        background: -webkit-linear-gradient(top, #ffffff 5%, #f6f6f6 100%);
        background: -o-linear-gradient(top, #ffffff 5%, #f6f6f6 100%);
        background: -ms-linear-gradient(top, #ffffff 5%, #f6f6f6 100%);
        background: linear-gradient(to bottom, #ffffff 5%, #f6f6f6 100%);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffff', endColorstr='#f6f6f6', GradientType=0);
        background-color: #ffffff;
        -moz-border-radius: 20%;
        -webkit-border-radius: 20%;
        border-radius: 20%;
        border: 1px solid #dcdcdc;
        display: inline-block;
        cursor: pointer;
        color: #666666;
        font-family: Arial;
        font-size: 15px;
        font-weight: bold;
        padding: 8px 24px;
        text-decoration: none;
        text-shadow: 0px 1px 0px #ffffff;

        position: fixed;
        top: 2%;
        left: 1.2%;
        z-index: 1;
    }

    .myButton:hover {
        background: -webkit-gradient(linear, left top, left bottom, color-stop(0.05, #f6f6f6), color-stop(1, #ffffff));
        background: -moz-linear-gradient(top, #f6f6f6 5%, #ffffff 100%);
        background: -webkit-linear-gradient(top, #f6f6f6 5%, #ffffff 100%);
        background: -o-linear-gradient(top, #f6f6f6 5%, #ffffff 100%);
        background: -ms-linear-gradient(top, #f6f6f6 5%, #ffffff 100%);
        background: linear-gradient(to bottom, #f6f6f6 5%, #ffffff 100%);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#f6f6f6', endColorstr='#ffffff', GradientType=0);
        background-color: #f6f6f6;
    }

    /*.myButton:active {
	position:relative;
	top:1px;
}
*/
</style>