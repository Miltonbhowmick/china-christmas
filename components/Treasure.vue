<template>
    <div class="treasure-box">
        <div class="money-box">
            <img src="/images/treasure-box.png" alt="treasure-box" />
        </div>
        <div class="header">
            <!-- <div class="title">金爺爺的大型老虎機</div> -->
            <div class="title">
                <div class="image">
                    <img src="/images/treasure-title.png" />
                </div>
            </div>

            <div class="leaflet">
                <div class="item">
                    <span class="value">遊戲平台特色與安全可靠</span>
                </div>
            </div>
            <div class="description">
                在金爺爺的大型老虎機，我們不僅提供絕佳的娛樂和豐富的故事，更重
                視玩家的遊戲體驗與安全。以下是我們平台的幾大特色和安全保障
            </div>
        </div>
        <div class="content">
            <div class="info">
                <div class="item">
                    <div class="overlap">
                        <div class="context">
                            <div class="left">
                                <!-- <div class="title">平台特色</div> -->
                                <div class="title">
                                    <div class="image">
                                        <img
                                            src="/images/treasure-title-1.png"
                                        />
                                    </div>
                                </div>
                            </div>
                            <div class="right">
                                <div class="context-item">
                                    <div class="title">多元化遊戲選擇</div>
                                    <p class="description">
                                        從經典老虎機到創新視頻老虎機
                                        ，應有盡有。每款遊戲都設計獨特
                                        ，搭配美輪美奐的圖形和迷人的
                                        聲音效果，確保每次旋轉都充滿 樂趣。
                                    </p>
                                </div>
                                <div class="context-item">
                                    <div class="title">個性化遊戲體驗</div>
                                    <p class="description">
                                        我們的平台提供個性化推薦，根
                                        據您的遊戲偏好和活動歷史推薦
                                        遊戲，讓您每次登入都有新發現
                                    </p>
                                </div>
                                <div class="context-item">
                                    <div class="title">即時客服支援</div>
                                    <p class="description">
                                        無論是技術問題還是遊戲疑問，
                                        我們的客服團隊��小時待命，確
                                        保您的遊戲體驗順暢無礙。
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="item">
                    <div class="overlap">
                        <div class="context">
                            <div class="left">
                                <!-- <div class="title">安全可靠</div> -->
                                <div class="title">
                                    <div class="image">
                                        <img
                                            src="/images/treasure-title-2.png"
                                        />
                                    </div>
                                </div>
                            </div>
                            <div class="right">
                                <div class="context-item">
                                    <div class="title">先進的加密技術</div>
                                    <p class="description">
                                        我們採用最先進的加密技術來
                                        保護您的個人信息和交易安全，
                                        確保您的數據在網上的安全不 受威脅。
                                    </p>
                                </div>
                                <div class="context-item">
                                    <div class="title">公平遊戲保證</div>
                                    <p class="description">
                                        使用認證的隨機數生成器（RNG）
                                        確保遊戲結果的公正性和隨機性
                                        。我們承諾提供100%公平的遊戲
                                        環境，讓每位玩家都有公平的勝 利機會。
                                    </p>
                                </div>
                                <div class="context-item">
                                    <div class="title">負責任的遊戲</div>
                                    <p class="description">
                                        我們致力於提供一個負責任的遊
                                        戲環境，享受健康的娛樂生活。
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="item">
                    <div class="overlap">
                        <div class="context">
                            <div class="left">
                                <!-- <div class="title">精選遊戲</div> -->
                                <div class="title">
                                    <div class="image">
                                        <img
                                            src="/images/treasure-title-3.png"
                                        />
                                    </div>
                                </div>
                            </div>
                            <div class="right">
                                <ul class="coin-list">
                                    <li
                                        v-for="(data, index) in coinData"
                                        :key="index"
                                    >
                                        <div class="coin-icon">
                                            <img
                                                :src="data.imageSrc"
                                                :alt="data.title"
                                            />
                                        </div>
                                        <div class="title">
                                            {{ data.title }}
                                        </div>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="move-box"><button class="btn">加入冒險</button></div>
        </div>
    </div>
</template>

<script setup>
const coinData = [
    {
        imageSrc: "/images/coin1.png",
        title: "十三張",
    },
    {
        imageSrc: "/images/coin2.png",
        title: "水果機",
    },
    {
        imageSrc: "/images/coin3.png",
        title: "牛牛",
    },
    {
        imageSrc: "/images/coin4.png",
        title: "炸金花",
    },
    {
        imageSrc: "/images/coin5.png",
        title: "賽馬",
    },
    {
        imageSrc: "/images/coin6.png",
        title: "鬥地主",
    },
    {
        imageSrc: "/images/coin7.png",
        title: "龍虎",
    },
];
</script>

<style scoped lang="scss">
.treasure-box {
    width: 100%;
    position: relative;
    .money-box {
        margin-top: -10rem;
        position: absolute;
        top: 0;
        left: 3%;
        width: 20%;
    }
    .header {
        margin-top: 5rem;
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        .title {
            margin-bottom: 20px;
            font-size: 40px;
            font-weight: 600;
            background: var(--primary-title-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: flex;
            justify-content: center;
            .image {
                width: 50%;
            }
        }
        .leaflet {
            margin-top: -30px;
            position: relative;
            width: 100%;
            display: flex;
            justify-content: center;
            .item {
                width: 30%;
                height: 50px;
                padding: 4px 4px 0px 4px;
                clip-path: polygon(
                    0 10px,
                    10px 0,
                    100% 0,
                    100% calc(100% - 10px),
                    calc(100% - 10px) 100%,
                    0 100%
                );
                background: var(--primary-title-gradient);
                .value {
                    width: 100%;
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    font-size: 30px;
                    color: #000;
                    font-weight: 400;
                    text-align: center;
                }
            }
        }
        .description {
            margin-top: 2rem;
            width: 30%;
            font-size: 14px;
            text-align: center;
        }
    }
    .content {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        .info {
            padding: 3rem 0;

            width: 80%;
            display: flex;
            flex-direction: column;
            gap: 40px;

            .item {
                padding: 4px 4px 4px 4px;
                height: 100%;
                width: 100%;
                border-radius: 25px;
                background: var(--primary-title-gradient);

                position: relative;
                .overlap {
                    padding: 10px 0;
                    display: flex;
                    justify-content: center;
                    position: relative;
                    min-height: 200px;
                    width: 100%;
                    background: linear-gradient(
                        90deg,
                        rgba(60, 60, 59, 1) 0%,
                        rgba(27, 0, 1, 1) 99.9181%
                    );
                    border-radius: 25px;
                    .context {
                        width: 100%;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        gap: 10px;
                        .left {
                            height: 15rem;
                            width: 10%;
                            display: flex;
                            justify-content: center;
                            align-items: center;
                            writing-mode: vertical-lr;
                            .title {
                                text-orientation: mixed;
                                font-size: 30px;
                                font-weight: 600;
                                background: var(--primary-title-gradient);
                                -webkit-background-clip: text;
                                -webkit-text-fill-color: transparent;
                                display: flex;
                                align-items: center;
                                .image {
                                    // width: 30%;
                                }
                            }
                        }
                        .right {
                            width: 85%;
                            display: flex;
                            justify-content: space-between;
                            align-items: flex-start;
                            .context-item {
                                width: 30%;
                                display: flex;
                                flex-direction: column;
                                align-items: center;
                                .title {
                                    margin-top: -10px;
                                    font-size: 20px;
                                    font-weight: 600;
                                    background: var(--primary-title-gradient);
                                    -webkit-background-clip: text;
                                    -webkit-text-fill-color: transparent;
                                }
                                .description {
                                    font-size: 18px;
                                    color: #fff;
                                    text-align: center;
                                }
                            }
                            .coin-list {
                                list-style: none;
                                margin: 0;
                                padding: 0;
                                display: flex;
                                justify-content: space-between;
                                gap: 20px;
                                li {
                                    display: flex;
                                    flex-direction: column;
                                    align-items: center;
                                    .coin-icon {
                                        // width: 70%;
                                    }
                                    .title {
                                        margin-top: -10px;
                                        font-size: 25px;
                                        font-weight: 600;
                                        background: var(
                                            --primary-title-gradient
                                        );
                                        -webkit-background-clip: text;
                                        -webkit-text-fill-color: transparent;
                                    }
                                }
                            }
                        }
                    }
                }
            }

            // .item {
            //     padding: 10px;
            //     height: 265px;
            //     width: 100%;
            //     background-image: url("/images/rounded-box.png");
            //     background-repeat: no-repeat;
            //     background-size: cover;
            //     display: flex;
            //     justify-content: center;
            //     align-items: center;
            //     .left {
            //         height: 60%;
            //         width: 20%;
            //         display: flex;
            //         justify-content: center;
            //         align-items: center;
            //         writing-mode: vertical-lr;
            //         .title {
            //             text-orientation: mixed;
            //             font-size: 30px;
            //             font-weight: 600;
            //             background: var(--primary-title-gradient);
            //             -webkit-background-clip: text;
            //             -webkit-text-fill-color: transparent;
            //         }
            //     }
            //     .right {
            //         height: 60%;
            //         width: 70%;
            //         display: flex;
            //         justify-content: space-between;
            //         align-items: flex-start;
            //         .context-item {
            //             width: 30%;
            //             display: flex;
            //             flex-direction: column;
            //             align-items: center;
            //             .title {
            //                 margin-top: -10px;
            //                 font-size: 30px;
            //                 font-weight: 600;
            //                 background: var(--primary-title-gradient);
            //                 -webkit-background-clip: text;
            //                 -webkit-text-fill-color: transparent;
            //             }
            //             .description {
            //                 font-size: 18px;
            //                 color: #fff;
            //                 text-align: center;
            //             }
            //         }
            //         .coin-list {
            //             list-style: none;
            //             margin: 0;
            //             padding: 0;
            //             display: flex;
            //             justify-content: space-between;
            //             gap: 20px;
            //             li {
            //                 display: flex;
            //                 flex-direction: column;
            //                 align-items: center;
            //                 .coin-icon {
            //                     // width: 70%;
            //                 }
            //                 .title {
            //                     margin-top: -10px;
            //                     font-size: 25px;
            //                     font-weight: 600;
            //                     background: var(--primary-title-gradient);
            //                     -webkit-background-clip: text;
            //                     -webkit-text-fill-color: transparent;
            //                 }
            //             }
            //         }
            //     }
            // }
        }
        .move-box {
            width: 235px;
            height: 60px;
            padding-bottom: 45px;
            .btn {
                border: none;
                height: 100%;
                width: 100%;
                border-radius: 10px;
                background: var(--primary-gradient-bg);
                font-size: 30px;
                font-weight: 400;
                cursor: pointer;
            }
        }
    }
}
</style>
