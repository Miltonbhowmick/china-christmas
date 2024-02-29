<template>
    <div class="meeting-box">
        <div class="header">
            <div class="title">
                <img src="/images/meeting-title.png" />
            </div>
        </div>
        <div class="content"></div>
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
            // margin-top: 1rem;
            width: 25%;
        }
    }
    .content {
        height: 100%;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }
}
</style>
