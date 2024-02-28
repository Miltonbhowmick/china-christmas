<template>
    <header class="header">
        <div class="cap-box">
        </div>
        <div class="head-box">
            <div class="logo">
                <a class="company-link"
                    ><img src="/images/company-logo.png" alt="company-logo"
                /></a>
               
            </div>
            <div class="header-nav-links">
                <div class="nav-item">
                    <img class="bg" src="/images/yellow-nav-item-bg.png" alt="red-nav-item-bg"/>
                    <span class="title text-black">Milton</span>
                </div>
                <div class="nav-item">
                    <img class="bg" src="/images/red-nav-item-bg.png" alt="red-nav-item-bg"/>
                    <span class="title">Milton</span>
                </div>
                <div class="nav-item">
                    <img class="bg" src="/images/red-nav-item-bg.png" alt="red-nav-item-bg"/>
                    <span class="title">Milton</span>
                </div>
                <div class="nav-item">
                    <img class="bg" src="/images/red-nav-item-bg.png" alt="red-nav-item-bg"/>
                    <span class="title">Milton</span>
                </div>
            </div>
        </div>
    </header>
</template>

<script setup>
import redNavItem from "~/assets/images/red-nav-item-bg.png"

</script>

<style scoped lang="scss">
.header {
    height: 50px;
    position: relative;
    .cap-box{
        height: 100%;
        background-image: url('/images/cap-box.png');
    }
    .head-box {
        margin-top: -8px;
        height: 100%;
        box-sizing: border-box;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        // background: #191919;
        // min-width: 1100px;
        padding: 0 10%;
        .logo {
            margin-top: 32px;
            height: 235%;
            a {
                // display: block;
                // padding: 2px 20px 2px 0;
                // height: 40px;
            }
        }
        .header-nav-links {
            height: 100%;
            display: flex;
            align-items: center;
            gap: 5px;
            .nav-item{
                position: relative;
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: center;
                .bg{

                }
                .title{
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    font-size: 20px;
                }
            }

        }
    }

    @media (max-width: 768px) {
        display: none;
    }
}

</style>
