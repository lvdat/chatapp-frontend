<template>
    <NavigationHome />
    <div class="container mt-3 landing-container">
        <div class="row">
            <div class="col-md-6">
                <LandingText />
                <LoginForm v-if="login" />
                <p v-if="login">
                    Bạn chưa có tài khoản?, <a class="change-state_link" @click="changeState">Đăng ký ngay!</a>
                </p>
                <p v-else>
                    Bạn đã có tài khoản?, <a class="change-state_link" @click="changeState">Đăng nhập ngay!</a>
                </p>
            </div>
            <div class="col-md-6">
                <LandingImage />

            </div>
        </div>
    </div>
</template>
<script>
import NavigationHome from '@/components/NavigationHome.vue'
import LandingText from '@/components/LandingText.vue'
import LandingImage from '@/components/LandingImage.vue'
import LoginForm from '@/components/LoginForm.vue'

export default {
    components: {
        NavigationHome,
        LandingText,
        LandingImage,
        LoginForm,
    },
    data () {
        return {
            login: true,
        }
    },
    methods: {
        changeState () {
            const currentState = this.login
            this.login = !currentState
        }
    }
}
</script>
<style>
.landing-container {
    padding-top: 50px;
}
.change-state_link {
    text-decoration: none;
    cursor: pointer;
}
</style>