<template>
    <div class="meeting-box">
        <div class="header">
            <!-- <div class="title">遊戲豐富</div> -->
            <div class="title">
                <div class="image"><img src="/images/meeting-title.png" /></div>
            </div>
        </div>
        <div class="content">
            <div class="info">
                <div class="mega-news">
                    <div class="item">
                        <div class="overlap">
                            <div class="context">
                                <p class="description">
                                    在金爺爺的娱乐老虎機，您將找到結合傳統老虎機機制和迷人故事的
                                    遊戲陣容。每支遊戲老虎機都講述了金爺爺故事的一部分，從他的卑微
                                    開始到他成為運氣皇帝的崛起。冒險進入龍之巢尋找火熱的財富，探索
                                    絲綢旋轉品味奢華，或潛入神秘月光尋找隱藏的寶藏
                                </p>
                            </div>
                        </div>
                    </div>
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
            display: flex;
            justify-content: center;
            .image {
                width: 60%;
            }
        }
    }
    .content {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        .info {
            display: flex;
            justify-content: center;
            .mega-news {
                width: 50%;
                margin-top: 7rem;
                .item {
                    padding: 4px 4px 0px 4px;
                    height: 100%;
                    width: 100%;
                    // background-image: url("/images/timeline-item-box.png");
                    // background-repeat: no-repeat;
                    // background-size: cover;
                    // background-position: center center;
                    clip-path: polygon(
                        0 50px,
                        50px 0,
                        100% 0,
                        100% calc(100% - 50px),
                        calc(100% - 50px) 100%,
                        0 100%
                    );
                    background: var(--primary-title-gradient);

                    position: relative;
                    .overlap {
                        padding: 30px 0;
                        display: flex;
                        justify-content: center;
                        position: relative;
                        min-height: 120px;
                        width: 100%;
                        background: linear-gradient(
                            90deg,
                            rgba(60, 60, 59, 1) 0%,
                            rgba(27, 0, 1, 1) 99.9181%
                        );
                        clip-path: polygon(
                            0 50px,
                            50px 0,
                            100% 0,
                            100% calc(100% - 50px),
                            calc(100% - 50px) 100%,
                            0 100%
                        );

                        .context {
                            width: 80%;
                            // position: absolute;
                            // top: 10%;
                            // left: 15%;
                            display: flex;
                            flex-direction: column;
                            justify-content: center;
                            align-items: flex-start;
                            gap: 10px;
                            .title {
                                margin: 0 0 20px 0;
                                font-size: 40px;
                                font-weight: 600;
                                background: var(--primary-title-gradient);
                                -webkit-background-clip: text;
                                -webkit-text-fill-color: transparent;
                                text-align: center;
                            }
                            .description {
                                margin: 0;
                                font-size: 20px;
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>
