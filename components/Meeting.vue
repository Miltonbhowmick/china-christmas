<template>
    <div class="meeting-box">
        <div class="header">
            <div class="title">遊戲豐富</div>
        </div>
        <div class="content">
            <div class="info">
                <div class="mega-news">
                    <div class="bg">
                        <img
                            src="/images/focus-text-bg.png"
                            alt="focus-text-bg"
                        />
                    </div>
                    <span class="value"
                        >在金爺爺的娱乐老虎機，您將找到結合傳統老虎機機制和迷人故事的
                        遊戲陣容。每支遊戲老虎機都講述了金爺爺故事的一部分，從他的卑微
                        開始到他成為運氣皇帝的崛起。冒險進入龍之巢尋找火熱的財富，探索
                        絲綢旋轉品味奢華，或潛入神秘月光尋找隱藏的寶藏。</span
                    >
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.meeting-box {
    background-image: url("/images/meeting-bg.png");
    background-size: cover;
    background-repeat: no-repeat;
    height: 80vh;
    width: 100%;
    .header {
        width: 100%;
        display: flex;
        justify-content: center;
        .title {
            font-size: 6rem;
            font-weight: 600;
            background: var(--primary-title-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    }
    .content {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        .info {
            .mega-news {
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
                    font-size: 25px;
                    font-weight: 500;
                    color: #fff;
                }
            }
        }
    }
}
</style>
