<template>
    <section class="timeline">
        <div class="header">
            <!-- <h2 class="title">遊戲介紹</h2> -->
            <div class="title">
                <div class="image">
                    <img src="/images/hero-banner-title.png" />
                </div>
            </div>
        </div>

        <div class="content">
            <div class="info">
                <div
                    v-for="(data, index) in timelineDataList"
                    :key="'timeline_' + index"
                    class="box"
                >
                    <div class="coin-box">
                        <img :src="data.coinSrc" alt="coin1" />
                    </div>
                    <div class="item">
                        <div class="overlap">
                            <div class="context">
                                <!-- <h4 class="title">{{ data.title }}</h4> -->
                                <div class="title">
                                    <div class="image">
                                        <img :src="data.titleImage" />
                                    </div>
                                </div>
                                <div class="description-box">
                                    <p
                                        v-for="(
                                            desObj, idx
                                        ) in data.descriptionList"
                                        :key="'desc_' + idx"
                                        class="description"
                                    >
                                        <span
                                            v-if="desObj.colorValue"
                                            class="bg-color"
                                            >{{ desObj.colorValue }}</span
                                        ><span>{{ desObj.value }}</span>
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
let timelineDataList = [
    {
        coinSrc: "/images/coin1.png",
        title: "十三張遊戲",
        titleImage: "/images/timeline-1-title.png",
        descriptionList: [
            {
                colorValue: null,
                value: "十三支是一種撲克遊戲，使用撲克牌型，盛行於華人地區。常稱之為華人撲克（Chinese Poker）、羅宋，撲克遊戲的一種，盛行於華人地區",
            },
            {
                colorValue: "玩法介紹",
                value: null,
            },
            {
                colorValue: null,
                value: "每局使用一副牌(不含大小王，共52張)，每名玩家分配13張牌。",
            },
            {
                colorValue: null,
                value: "將13張牌擺成三墩(頭墩3張，中墩、尾墩各5張)",
            },
            {
                colorValue: null,
                value: "頭墩必須小於中墩，中墩必須小於尾墩，否則則為“倒水",
            },
            {
                colorValue: "牌型",
                value: "同花順>鐵支>葫蘆>同花>順子>三條>兩對>對子>烏龍",
            },
            {
                colorValue: "點數",
                value: "A>K>Q>J>10>9>8>7>6>5>4>3>2",
            },
            {
                colorValue: "特殊牌型:",
                value: "至尊青龍>一條龍>十二皇族>三同花順>三分天下>全大>全小>湊一色>四套三條>五對三條> 六對半>三順子>三同花",
            },
        ],
    },
    {
        coinSrc: "/images/coin6.png",
        title: "十三張遊戲",
        titleImage: "/images/timeline-2-title.png",
        descriptionList: [
            {
                colorValue: null,
                value: "十三支是一種撲克遊戲，使用撲克牌型，盛行於華人地區。常稱之為華人撲克（Chinese Poker）、羅宋，撲克遊戲的一種，盛行於華人地區",
            },
            {
                colorValue: "玩法介紹",
                value: null,
            },
            {
                colorValue: null,
                value: "每局使用一副牌(不含大小王，共52張)，每名玩家分配13張牌。",
            },
            {
                colorValue: null,
                value: "將13張牌擺成三墩(頭墩3張，中墩、尾墩各5張)",
            },
            {
                colorValue: null,
                value: "頭墩必須小於中墩，中墩必須小於尾墩，否則則為“倒水",
            },
            {
                colorValue: "牌型",
                value: "同花順>鐵支>葫蘆>同花>順子>三條>兩對>對子>烏龍",
            },
            {
                colorValue: "點數",
                value: "A>K>Q>J>10>9>8>7>6>5>4>3>2",
            },
            {
                colorValue: "特殊牌型:",
                value: "至尊青龍>一條龍>十二皇族>三同花順>三分天下>全大>全小>湊一色>四套三條>五對三條> 六對半>三順子>三同花",
            },
        ],
    },
];
</script>

<style scoped lang="scss">
section.timeline {
    margin-top: 100px;
    .header {
        .title {
            font-size: 60px;
            font-weight: 600;
            background: var(--primary-title-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-align: center;
            display: flex;
            justify-content: center;
            .image {
                width: 20%;
            }
        }
    }
    .content {
        padding: 30px 0 50px 0;
        display: flex;
        justify-content: center;

        .info {
            width: 70%;
            display: flex;
            flex-direction: column;
            gap: 50px;
            .box {
                position: relative;
                .coin-box {
                    z-index: 99;
                    width: 20%;
                    position: absolute;
                    top: 55%;
                    left: -10%;
                    transform: translateY(-50%);
                }
            }
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
                    padding: 50px 0;
                    display: flex;
                    justify-content: center;
                    position: relative;
                    min-height: 300px;
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
                        width: 70%;
                        // position: absolute;
                        // top: 10%;
                        // left: 15%;
                        display: flex;
                        flex-direction: column;
                        align-items: flex-start;
                        gap: 10px;
                        .title {
                            margin: 0 0 20px 0;
                            font-size: 40px;
                            font-weight: 600;
                            background: var(--primary-title-gradient);
                            -webkit-background-clip: text;
                            -webkit-text-fill-color: transparent;
                            display: flex;
                            justify-content: flex-start;
                            .image {
                                width: 40%;
                            }
                        }
                        .description-box {
                            margin-top: -2rem;
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
.bg-color {
    color: rgba(248, 222, 123, 1);
}
</style>

