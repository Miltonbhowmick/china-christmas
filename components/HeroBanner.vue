<template>
    <div class="hero-box">
        <div class="content">
            <div class="mega-info">
                <div class="title">
                    <img
                        src="/images/hero-banner-title.png"
                        alt="hero-banner-mid-title"
                    />
                </div>
                <div class="mid-title mt-negative-30">
                    <img
                        src="/images/hero-banner-mid-title.png"
                        alt="hero-banner-mid-title"
                    />
                </div>
                <div class="christmas-man">
                    <img src="/images/christmas-man.png" alt="christmas-man" />
                </div>
            </div>
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
        justify-content: center;
        .mega-info {
            margin-top: 30px;
            width: 50%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            gap: 0px;
            .title {
                width: 50%;
            }
            .mid-title {
                width: 70%;
            }
            .christmas-man {
                width: 70%;
            }
        }
    }
}

.mt-negative-30 {
    margin-top: -30px;
}
</style>
