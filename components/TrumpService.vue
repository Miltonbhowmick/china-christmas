<template>
    <div class="trump-service-box">
        <div class="header">
            <!-- <div class="title">為什麼在這裡玩？</div> -->
            <div class="title">
                <div class="image"><img src="/images/trump-title.png" /></div>
            </div>
        </div>
        <div class="content">
            <div class="info">
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/flower.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">
                        體驗遊戲的刺激感，擁有金爺爺本人的祝福。我
                        們獨特的算法確保每次旋轉都是新的財富機會。
                    </div>
                </div>
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/Asset 85.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">
                        沉浸在這片土地的傳說中。我們平台上的每個遊
                        戲都講述一個故事，使您通往財富的旅程成為一
                        次史詩般的冒險
                    </div>
                </div>
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/Asset 84.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">
                        忠誠值得認可。我們的獎勵計劃確保您探索得越
                        多，獎勵就越豐富。專屬紅利、免費旋轉和秘密遊
                        戲等待著我們最冒險的玩家
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.trump-service-box {
    background-image: url("/images/trump-bg.png");
    background-size: cover;
    background-repeat: no-repeat;
    height: 120vh;
    width: 100%;
    .header {
        width: 100%;
        display: flex;
        justify-content: center;
        .title {
            margin-top: 10rem;
            font-size: 40px;
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
        align-items: flex-start;
        .info {
            margin-top: 100px;
            width: 40%;
            display: flex;
            flex-direction: column;
            justify-content: flex-start;
            align-items: flex-start;
            .item {
                display: flex;
                align-items: center;
                gap: 20px;
                .sign-image {
                    width: 15%;
                }
                .icon {
                    width: 25%;
                }
                .description {
                    width: 60%;
                    font-size: 16px;
                }
            }
        }
    }
}
</style>
