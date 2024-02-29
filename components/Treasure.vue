<template>
    <div class="treasure-box">
        <div class="money-box">
            <img src="/images/treasure-box.png" alt="treasure-box" />
        </div>
        <div class="header">
            <div class="title">
                <img src="/images/treasure-title.png" alt="title" />
            </div>
            <div class="leaflet">
                <img src="/images/treasure-leaflet.png" alt="leaflet" />
            </div>
            <div class="description">aniosdiasdnoiasndoiasndaosndasoidnoi</div>
        </div>
        <div class="content">
            <div class="info">
                <div class="item">
                    <div class="left">
                        <div class="title">
                            <img src="/images/treasure-item-title1.png" />
                        </div>
                    </div>
                    <div class="right">
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                從經典老虎機到創新視頻老虎機
                                ，應有盡有。每款遊戲都設計獨特
                                ，搭配美輪美奐的圖形和迷人的
                                聲音效果，確保每次旋轉都充滿 樂趣。
                            </p>
                        </div>
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                我們的平台提供個性化推薦，根
                                據您的遊戲偏好和活動歷史推薦
                                遊戲，讓您每次登入都有新發現
                            </p>
                        </div>
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                無論是技術問題還是遊戲疑問，
                                我們的客服團隊��小時待命，確
                                保您的遊戲體驗順暢無礙。
                            </p>
                        </div>
                    </div>
                </div>
                <div class="item">
                    <div class="left">
                        <div class="title">
                            <img src="/images/treasure-item-title1.png" />
                        </div>
                    </div>
                    <div class="right">
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                我們採用最先進的加密技術來
                                保護您的個人信息和交易安全，
                                確保您的數據在網上的安全不 受威脅。
                            </p>
                        </div>
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                使用認證的隨機數生成器（RNG）
                                確保遊戲結果的公正性和隨機性
                                。我們承諾提供���%公平的遊戲
                                環境，讓每位玩家都有公平的勝 利機會。
                            </p>
                        </div>
                        <div class="context-item">
                            <div class="title">
                                <img
                                    src="/images/context-item-title-1.png"
                                    alt="context-item-title-1"
                                />
                            </div>
                            <p class="description">
                                我們致力於提供一個負責任的遊
                                戲環境，享受健康的娛樂生活。
                            </p>
                        </div>
                    </div>
                </div>
                <div class="item">
                    <div class="left">
                        <div class="title">
                            <img src="/images/treasure-item-title1.png" />
                        </div>
                    </div>
                    <div class="right">
                        <ul class="coin-list">
                            <li>
                                <div class="coin-icon">
                                    <img src="/images/coin1.png" alt="coin1" />
                                </div>
                                <div class="title">
                                    <img
                                        src="/images/coin-title1.png"
                                        alt="context-item-title-1"
                                    />
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="move-box"><button class="btn">加入冒險</button></div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.treasure-box {
    width: 100%;
    position: relative;
    .money-box {
        margin-top: -10rem;
        position: absolute;
        top: 0;
        left: 10%;
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
            width: 25%;
        }
        .leaflet {
            width: 500px;
        }
        .description {
            margin-top: 3rem;
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

            .item {
                padding: 10px;
                height: 265px;
                width: 100%;
                background-image: url("/images/rounded-box.png");
                background-repeat: no-repeat;
                background-size: cover;
                display: flex;
                justify-content: center;
                align-items: center;
                .left {
                    height: 60%;
                    width: 20%;
                    display: flex;
                    justify-content: center;
                    .title {
                        width: 35%;
                    }
                }
                .right {
                    height: 60%;
                    width: 70%;
                    display: flex;
                    justify-content: space-between;
                    align-items: flex-start;
                    .context-item {
                        width: 30%;
                        display: flex;
                        flex-direction: column;
                        align-items: flex-start;
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
                        gap: 10px;
                        li {
                            display: flex;
                            flex-direction: column;
                            align-items: center;
                            .coin-icon {
                                width: 100px;
                            }
                            .title {
                                margin-top: -10px;
                                width: 70%;
                            }
                        }
                    }
                }
            }
        }
        .move-box {
            width: 235px;
            height: 60px;
            padding-bottom: 45px;
            .btn {
                height: 100%;
                width: 100%;
                background-image: url("/images/move-btn-bg.png");
                background-repeat: no-repeat;
                background-size: cover;
            }
        }
    }
}
</style>
