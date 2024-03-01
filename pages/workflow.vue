<template>
    <section class="workflow">
        <div class="header">
            <!-- <h2 class="title">操作指南</h2> -->
            <div class="title">
                <div class="image">
                    <img src="/images/workflow-title.png" />
                </div>
            </div>
        </div>

        <div class="mega-news">
            <div class="box">
                <div class="item">
                    <div class="overlap">
                        <div class="context">
                            <h4 class="title">
                                歡迎來到金爺爺的大型老虎機：快速開始指南
                            </h4>
                            <p class="description">
                                在金爺爺的大型老虎機，我們致力於提供一個無縫且享受的遊戲體驗。以下
                                是快速開始遊戲的簡單步驟
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="data-flow">
            <div class="head-box"><h3>註冊成為會員</h3></div>
            <div class="flow-content">
                <div class="item">
                    <div class="icon-box">
                        <img src="/images/Asset 49.png" alt="Asset 49" />
                    </div>
                    <h3 class="title">訪問註冊頁面</h3>
                    <p class="notices">
                        首先，請訪問我們的網 站並點擊「註冊」按鈕。
                    </p>
                </div>
                <div class="item w-10">
                    <div class="arrow-sign">
                        <img src="/images/Asset 52.png" alt="Asset 50" />
                    </div>
                </div>
                <div class="item">
                    <div class="icon-box">
                        <img src="/images/Asset 50.png" alt="Asset 50" />
                    </div>
                    <h3 class="title">填寫個人資料</h3>
                    <p class="notices">
                        在註冊表單中輸入您的姓 名、電話號碼、身份證字型
                        大小（為了確保您的年齡 符合遊戲要求）以及您的
                        電子郵件地址。
                    </p>
                </div>
                <div class="item w-10">
                    <div class="arrow-sign">
                        <img src="/images/Asset 52.png" alt="Asset 50" />
                    </div>
                </div>
                <div class="item">
                    <div class="icon-box">
                        <img src="/images/Asset 51.png" alt="Asset 51" />
                    </div>
                    <h3 class="title">完成註冊</h3>
                    <p class="notices">
                        核對您的資料無誤後， 點擊「提交」完成註冊過
                        程。您將收到一封確認 郵件，請按照郵件中的
                        指示�動您的帳號
                    </p>
                </div>
            </div>
        </div>

        <div class="christmas-idea">
            <div class="info">
                <div class="data-box">
                    <div class="head-box"><h3>開始遊戲</h3></div>
                    <p class="description">
                        一旦您的帳號被�動，您就可以立即開始探索金爺爺的大型老虎機的精彩
                        世界了！從經典老虎機到最新遊戲，這裡應有盡有，滿足您的遊戲需求
                    </p>
                </div>
                <div class="data-box">
                    <div class="head-box"><h3>客服支援</h3></div>
                    <p class="description">
                        如果在註冊過程中或遊戲過程中遇到任何問題，請不要猶豫，立即聯繫我們的客
                        服團隊。我們的客服支援團隊全天候在線，隨時準備回答您的疑問並提供幫助。
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
section.workflow {
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
    .mega-news {
        display: flex;
        justify-content: center;
        .box {
            width: 45%;
            position: relative;
            .coin-box {
                z-index: 99;
                width: 20%;
                position: absolute;
                top: 55%;
                left: -10%;
                transform: translateY(-50%);
            }
            .item {
                padding: 4px 4px 0px 4px;
                height: 100%;
                width: 100%;
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
                    padding: 40px 0;
                    display: flex;
                    justify-content: center;
                    position: relative;
                    min-height: 100px;
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
                        width: 85%;
                        display: flex;
                        flex-direction: column;
                        align-items: flex-start;
                        gap: 10px;
                        .title {
                            margin: 0 0 10px 0;
                            font-size: 20px;
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
    .data-flow {
        background-image: url("/images/Asset 57.png");
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        padding: 15rem 0;

        .head-box {
            width: 28%;
            height: 70px;

            background: var(--primary-title-gradient);
            clip-path: polygon(
                0 10px,
                10px 0,
                100% 0,
                100% calc(100% - 10px),
                calc(100% - 10px) 100%,
                0 100%
            );
            display: flex;
            justify-content: center;
            align-items: center;
            h3 {
                color: #000;
                font-size: 40px;
                font-weight: 400;
            }
        }
        .flow-content {
            width: 70%;
            margin-top: 3rem;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            gap: 10px;
            .item {
                width: 33%;
                height: 100%;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                &.w-10 {
                    width: 10%;
                }
                .icon-box {
                    margin-left: 30px;
                    width: 50%;
                }
                .arrow-sign {
                    margin-top: 34px;
                }
                .title {
                    margin: 0;
                    font-size: 18px;
                    font-weight: 600;
                    background: var(--primary-title-gradient);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                    text-align: center;
                }
                .notices {
                    width: 80%;
                    font-size: 20px;
                    text-align: center;
                }
            }
        }
    }
    .christmas-idea {
        margin-top: -15rem;
        background-image: url("/images/Asset 54.png");
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 110vh;
        .info {
            display: flex;
            flex-direction: column;
            gap: 60px;
            .data-box {
                display: flex;
                flex-direction: column;
                align-items: center;
                .head-box {
                    width: 28%;
                    height: 70px;
                    background: var(--primary-title-gradient);
                    clip-path: polygon(
                        0 10px,
                        10px 0,
                        100% 0,
                        100% calc(100% - 10px),
                        calc(100% - 10px) 100%,
                        0 100%
                    );
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    h3 {
                        color: #000;
                        font-size: 30px;
                        font-weight: 400;
                    }
                }
                .description {
                    width: 40%;
                    text-align: center;
                    font-size: 25px;
                }
            }
        }
    }
}
</style>
