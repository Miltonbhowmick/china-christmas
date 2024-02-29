<template>
    <div class="trump-service-box">
        <div class="header">
            <div class="title">
                <img src="/images/trump-title.png" />
            </div>
        </div>
        <div class="content">
            <div class="info">
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/flower.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">asmdomamsdaosdmasd</div>
                </div>
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/flower.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">asmdomamsdaosdmasd</div>
                </div>
                <div class="item">
                    <div class="sign-image">
                        <img src="/images/flower.png" />
                    </div>
                    <div class="icon"><img src="/images/lang-icon.png" /></div>
                    <div class="description">asmdomamsdaosdmasd</div>
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
            width: 30%;
        }
    }
    .content {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: flex-start;
        .info {
            display: flex;
            flex-direction: column;
            justify-content: flex-start;
            .item {
                display: flex;
                align-items: center;
                gap: 20px;
                .sign-image {
                    width: 20%;
                }
                .icon {
                    width: 30%;
                }
            }
        }
    }
}
</style>
