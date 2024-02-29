<template>
    <section class="signin">
        <div class="grad-box">
            <div class="auth-box">
                <div class="toggle-box">
                    <a
                        @click="toggleAuth = 0"
                        class="signin-btn"
                        :class="{ active: toggleAuth === 0 }"
                        >註冊</a
                    >
                    <a
                        @click="toggleAuth = 1"
                        class="signup-btn"
                        :class="{ active: toggleAuth === 1 }"
                        >註冊</a
                    >
                </div>
                <form class="form" v-if="toggleAuth === 0">
                    <p class="headline">
                        歡迎開始您的運氣之旅！請填寫以下表格以創建您的帳戶。
                    </p>
                    <div class="input-group">
                        <label class="label">姓名：</label>
                        <input type="email" placeholder="(請輸入您的全名)" />
                    </div>
                    <div class="input-group">
                        <label class="label">姓名：</label>
                        <input
                            type="text"
                            placeholder="(請輸入您的聯繫電話號碼)"
                        />
                    </div>
                    <div class="input-group">
                        <label class="label">身份證字號：</label>
                        <input
                            type="text"
                            placeholder="(請輸入您的身份證字號)"
                        />
                    </div>
                    <div class="input-group">
                        <label class="label">郵件地址：</label>
                        <input
                            type="text"
                            placeholder="(請輸入您的電子郵件地址)"
                        />
                    </div>
                    <button class="btn">註冊</button>
                    <p class="notice">登入（如果已經是會員）</p>
                </form>
                <form class="form" v-else-if="toggleAuth === 1">
                    <p class="headline">
                        歡迎回到金爺爺！請使用您的帳戶資訊登入，繼續您的運氣
                        之旅和探索更多精彩遊戲。
                    </p>
                    <div class="input-group">
                        <label class="label">郵件地址：</label>
                        <input
                            type="email"
                            placeholder="(請輸入您的電子郵件地址)"
                        />
                    </div>
                    <div class="input-group">
                        <label class="label">密碼：</label>
                        <input type="text" placeholder="(請輸入您的密碼)" />
                    </div>
                    <p class="notice">
                        忘記密碼？ (如果您忘記了密碼，請點擊此處重設)
                    </p>
                    <button class="btn">登入</button>
                    <p class="notice">還不是會員？立即註冊!</p>
                    <p class="notice">(加入我們，開�您的運氣之旅)</p>
                </form>
            </div>
        </div>
    </section>
</template>

<script setup>
var toggleAuth = ref(0);
</script>

<style scoped lang="scss">
section.signin {
    padding: 50px 0;
    display: flex;
    justify-content: center;
    .grad-box {
        margin-top: 4rem;
        width: 60%;
        padding: 4px;
        background: var(--primary-title-gradient);
        border-radius: 25px;
        padding: 5px 5px;
        .auth-box {
            width: 100%;
            height: 100%;
            border-radius: 25px;
            background: var(--secondary-gradient-bg);
            display: flex;
            flex-direction: column;
            align-items: center;
            .toggle-box {
                width: 40%;
                padding: 30px 0;
                display: flex;
                justify-content: space-between;
                gap: 50px;
                a {
                    font-size: 40px;
                    font-weight: 600;
                    background: var(--primary-title-gradient);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                    text-align: center;
                    height: 70px;
                    cursor: pointer;
                    &.active {
                        border-bottom: 5px solid rgba(248, 222, 123, 1);
                    }
                }
            }
            .form {
                width: 60%;
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 15px;
                .headline {
                    margin: 0;
                    font-size: 20px;
                    background: var(--primary-title-gradient);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                    text-align: center;
                }
                .input-group {
                    width: 70%;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    gap: 10px;
                    .label {
                        font-size: 20px;
                        background: var(--primary-title-gradient);
                        -webkit-background-clip: text;
                        -webkit-text-fill-color: transparent;
                        text-align: center;
                    }
                    input {
                        border-radius: 4px;
                        width: 100%;
                        height: 40px;
                        border: none;
                        text-align: center;
                    }
                }
                .btn {
                    margin-top: 30px;
                    border: none;
                    width: 40%;
                    // height: 70px;
                    color: #000;
                    font-size: 25px;
                    font-weight: 400;
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
                }
                .notice {
                    font-size: 14px;
                    margin-bottom: 30px;
                    background: var(--primary-title-gradient);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                    text-align: center;
                }
            }
        }
    }
}
</style>
