<template>
    <header class="header">
        <div class="cap-box"></div>
        <div class="head-box">
            <div class="logo">
                <nuxt-link to="/" class="company-link"
                    ><img src="/images/company-logo.png" alt="company-logo"
                /></nuxt-link>
            </div>
            <div class="header-nav-links">
                <nuxt-link to="/" class="nav-item">
                    <img
                        v-if="menuActive === 0"
                        class="bg"
                        src="/images/yellow-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <img
                        v-else
                        class="bg"
                        src="/images/red-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />

                    <span
                        class="title"
                        :class="[menuActive === 0 ? 'text-black' : 'white']"
                        >首頁</span
                    >
                </nuxt-link>
                <nuxt-link to="/timeline" class="nav-item">
                    <img
                        v-if="menuActive === 1"
                        class="bg"
                        src="/images/yellow-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <img
                        v-else
                        class="bg"
                        src="/images/red-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <span
                        class="title"
                        :class="[menuActive === 1 ? 'text-black' : 'white']"
                        >遊戲介紹</span
                    >
                </nuxt-link>
                <nuxt-link to="/workflow" class="nav-item">
                    <img
                        v-if="menuActive === 2"
                        class="bg"
                        src="/images/yellow-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <img
                        v-else
                        class="bg"
                        src="/images/red-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <span
                        class="title"
                        :class="[menuActive === 2 ? 'text-black' : 'white']"
                        >操作指南</span
                    >
                </nuxt-link>
                <nuxt-link to="/signin" class="nav-item">
                    <img
                        v-if="menuActive === 3"
                        class="bg"
                        src="/images/yellow-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <img
                        v-else
                        class="bg"
                        src="/images/red-nav-item-bg.png"
                        alt="red-nav-item-bg"
                    />
                    <span
                        class="title"
                        :class="[menuActive === 3 ? 'text-black' : 'white']"
                        >客服聯繫</span
                    >
                </nuxt-link>
                <div class="nav-item expand-50">
                    <div class="title">客服聯繫</div>
                </div>
            </div>
        </div>
    </header>
</template>

<script setup>
import redNavItem from "~/assets/images/red-nav-item-bg.png";

const route = useRoute();

var menuActive = computed(() => {
    if (route.path === "/") return 0;
    else if (route.path === "/timeline") return 1;
    else if (route.path === "/workflow") return 2;
    else if (route.path === "/signin") return 3;
});
</script>

<style scoped lang="scss">
.header {
    height: 50px;
    position: relative;
    .cap-box {
        height: 100%;
        background-image: url("/images/cap-box.png");
    }
    .head-box {
        margin-top: -8px;
        height: 100%;
        box-sizing: border-box;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        // background: #191919;
        // min-width: 1100px;
        padding: 0 10%;
        .logo {
            margin-top: 32px;
            height: 235%;
            a {
                // display: block;
                // padding: 2px 20px 2px 0;
                // height: 40px;
            }
        }
        .header-nav-links {
            height: 100%;
            display: flex;
            align-items: center;
            gap: 5px;
            .nav-item {
                position: relative;
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: center;
                &.expand-50 {
                    width: 140px;
                }
                .bg {
                }
                .title {
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    font-size: 16px;
                    &.white {
                        color: #fff;
                    }
                }
            }
        }
    }

    @media (max-width: 768px) {
        display: none;
    }
}
</style>
