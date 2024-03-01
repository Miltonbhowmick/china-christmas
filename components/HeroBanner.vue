<template>
    <div class="hero-box">
        <div class="content">
            <div class="mega-info">
                <!-- <div class="title">歡迎來到</div> -->
                <!-- <div class="mid-title mt-negative-30">金爺爺的大型老虎機！</div> -->
                <div class="title">
                    <div class="image">
                        <img src="/images/hero-banner-title.png" />
                    </div>
                </div>
                <div class="mid-title">
                    <div class="image">
                        <img src="/images/hero-banner-subtitle.png" />
                    </div>
                </div>
                <div class="christmas-man">
                    <img src="/images/christmas-man.png" alt="christmas-man" />
                </div>
            </div>
            <div class="mega-news">
                <div class="item">
                    <div class="overlap">
                        <div class="context">
                            <!-- <h4 class="title">{{ data.title }}</h4> -->
                            <p class="description">
                                進入金爺爺的世界，一位傳奇人物，他的運氣和繁榮已成為傳說。在數字城
                                市的心臟地帶隱藏著一顆寶石，這是通往一個世界的門戶，那裡的運氣和
                                財富對大膽者微笑。這不僅僅是任何賭場；這是由運氣大師金爺爺自己創建
                                的聖地
                            </p>
                        </div>
                    </div>
                </div>
            </div>
            <!-- <div class="mega-news">
                <div class="bg">
                    <img src="/images/focus-text-bg.png" alt="focus-text-bg" />
                </div>
                <span class="value"
                    >進入金爺爺的世界，一位傳奇人物，他的運氣和繁榮已成為傳說。在數字城
                    市的心臟地帶隱藏著一顆寶石，這是通往一個世界的門戶，那裡的運氣和
                    財富對大膽者微笑。這不僅僅是任何賭場；這是由運氣大師金爺爺自己創建
                    的聖地</span
                >
            </div> -->
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
                font-size: 3rem;
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
            .mid-title {
                margin-top: -40px;
                font-size: 2rem;
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
            .christmas-man {
                width: 70%;
            }
        }
        .mega-news {
            margin-top: -30px;
            width: 50%;
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
            .item {
                padding: 4px 4px 4px 4px;
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
                    padding: 20px 0;
                    display: flex;
                    justify-content: center;
                    position: relative;
                    min-height: 150px;
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
                        align-items: flex-start;
                        justify-content: center;
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
                            font-size: 18px;
                        }
                    }
                }
            }
        }
    }
}

.mt-negative-30 {
    margin-top: -30px;
}
</style>
