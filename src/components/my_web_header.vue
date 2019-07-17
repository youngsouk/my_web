<template>
    <div id="header">
        <div id = "header_start">
            <ul>
                <a href="https://github.com/youngsouk" target="_blank">
                    <li>

                        <img id="img" src="https://github.com/youngsouk.png">

                    </li>
                </a>
                <li>
                    <a href="https://youngsouk-hack.tistory.com/" target="_blank">
                        <img id="img" src="./../assets/Tistory.png">
                    </a>
                </li>

                <li>
                    <a href="https://github.com/st4nw" target="_blank">
                        <img id="img" src="https://github.com/st4nw.png">
                    </a>
                </li>

                <li>
                    <a href="http://c2w2m2.com/" target="_blank">
                        <img id="img" src="./../assets/c2w2m2.jpg">
                    </a>
                </li>

                <li>
                    <a href="https://m0nday.tistory.com/" target="_blank">
                        <img id="img" src="./../assets/m0nday.jpg">
                    </a>
                </li>

                <li>
                    <a href="https://github.com/ohboksa" target="_blank">
                        <img id="img" src="https://github.com/ohboksa.png">
                    </a>
                </li>

                <li>
                    <a href="https://github.com/junhoyeo" target="_blank">
                        <img id="img" src="https://github.com/junhoyeo.png">
                    </a>
                </li>

                <li>
                    <a href="https://github.com/SYWoo2003" target="_blank">
                        <img id="img" src="https://github.com/SYWoo2003.png">
                    </a>
                </li>
                
                <li>
                    <a href="https://github.com/harugatto" target="_blank">
                        <img id="img" src="https://github.com/harugatto.png">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css?family=Noto+Sans+HK&display=swap');

    #header {
        top: 0px;
        position: fixed;
        width: 100%;
        height: 8%;
        overflow: hidden;
        z-index: -1;
        background: linear-gradient(#addbd8, #add8e6);
    }

    #header_start{
        top: 0px;
        position: fixed;
        width: 100%;
        height: 8%;
        overflow: hidden;
        z-index: -1;
        overflow-x: auto;
        overflow-y : hidden;
        white-space: nowrap;
    }

    ul {
        list-style-type: none;
        font-family: 'Noto Sans HK', sans-serif;
        font-size: 20px;
        text-align: center;
        position: relative;
        height: 100%;
        width: 100%;
        text-align: center;
        margin: 0 0 0 0;
        padding: 0 0 0 0;
        text-align: center;
    }

    li {
        display: inline;
        margin: 0.9%;
        padding: 0 0 0 0;
    }

    #img {
        position: relative;
        top: 12%;
        height: 70%;
        border-radius: 50%;
        margin-right: 1.5%;
        margin-right: 1.5%;
        z-index: 2;
    }
</style>