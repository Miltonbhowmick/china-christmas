<template>
    <div class="service-box">
        <div class="content">
            <div class="info">
                <div class="title">
                    <img src="/images/service-headline.png" />
                </div>
                <div class="description">asdapsdnasodnasdnasdiasd</div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
.service-box {
    background-image: url("/images/services-bg.png");
    background-size: cover;
    background-repeat: no-repeat;
    height: 130vh;
    width: 100%;
    .content {
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
                width: 35%;
            }
        }
    }
}
</style>
