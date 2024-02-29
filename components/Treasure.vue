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
                                aniosdiasdnoiasndoiasndaosndasoidnoi
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
                                aniosdiasdnoiasndoiasndaosndasoidnoi
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
            <div class="move-box"><button class="btn">aaa</button></div>
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
                height: 250px;
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
                    width: 80%;
                    display: flex;
                    justify-content: space-between;
                    align-items: flex-start;
                    .context-item {
                        width: 30%;
                        display: flex;
                        flex-direction: column;
                        align-items: flex-start;
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
