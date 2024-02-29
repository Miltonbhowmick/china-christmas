<template>
    <div class="hero-box">
        <div class="content">
            <div class="mega-info">
                <div class="title">歡迎來到</div>
                <div class="mid-title mt-negative-30">金爺爺的大型老虎機！</div>
                <div class="christmas-man">
                    <img src="/images/christmas-man.png" alt="christmas-man" />
                </div>
            </div>
            <div class="mega-news">
                <div class="bg">
                    <img src="/images/focus-text-bg.png" alt="focus-text-bg" />
                </div>
                <span class="value"
                    >進入金爺爺的世界，一位傳奇人物，他的運氣和繁榮已成為傳說。在數字城
                    市的心臟地帶隱藏著一顆寶石，這是通往一個世界的門戶，那裡的運氣和
                    財富對大膽者微笑。這不僅僅是任何賭場；這是由運氣大師金爺爺自己創建
                    的聖地</span
                >
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.hero-box {
    margin-top: 100px;
    background-image: url("/images/hero-banner.png");
    // background-size: 100%;
    background-repeat: no-repeat;
    background-size: cover;
    height: 800px;
    width: 100%;
    .content {
        display: flex;
        flex-direction: column;
        align-items: center;
        .mega-info {
            z-index: 99;

            margin-top: 30px;
            width: 50%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            gap: 0px;
            .title {
                margin-bottom: 40px;
                font-size: 3rem;
                font-weight: 600;
                background: var(--primary-title-gradient);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }
            .mid-title {
                margin-bottom: 40px;
                font-size: 2rem;
                font-weight: 600;
                background: var(--primary-title-gradient);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }
            .christmas-man {
                width: 70%;
            }
        }
        .mega-news {
            margin-top: -30px;
            width: 45%;
            display: flex;
            justify-content: center;
            position: relative;
            .bg {
                // width: 0%;
            }
            .value {
                width: 80%;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                font-size: 18px;
                font-weight: 500;
                color: #fff;
            }
        }
    }
}

.mt-negative-30 {
    margin-top: -30px;
}
</style>
