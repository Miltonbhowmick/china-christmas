<template>
    <div class="service-box">
        <div class="content">
            <div class="info">
                <div class="title">我們的故事</div>
                <div class="description">
                    金爺爺曾是古絲綢之路岸邊的一名謙虛漁夫，一個月光皎潔的夜晚，他
                    捕獲了一條金鯉，這條魚變成了一枚神秘的硬幣。這枚硬幣上鑄有難得
                    一見的雙龍徽章，是通往無盡財富和無窮運氣的鑰匙。現在，金爺爺邀
                    請您來測試您的命運，旋轉飾有幸運符號的轉輪，看看大師的運氣是否
                    也流經您的身體
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.service-box {
    background-image: url("/images/service-bg-2.png");
    background-size: cover;
    background-repeat: no-repeat;
    height: 130vh;
    width: 100%;
    display: flex;
    justify-content: center;
    .content {
        width: 80%;
        height: 100%;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        .info {
            margin-top: 4rem;
            width: 50%;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            .title {
                margin-bottom: 10px;
                font-size: 2.5rem;
                font-weight: 600;
                background: var(--primary-title-gradient);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }
            .description {
                font-size: 18px;
            }
        }
    }
}
</style>
