<template>
    <NavigationHome />
    <div class="container mt-3 landing-container">
        <div class="row">
            <div class="col-md-6">
                <LandingText />
            </div>
            <div class="col-md-6">
                <div class="card">
                    <div class="card-body">
                        A
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import NavigationHome from '@/components/NavigationHome.vue'
import LandingText from '@/components/LandingText.vue'

export default {
    components: {
        NavigationHome,
        LandingText,
    }
}
</script>
<style>
.landing-container {
    padding-top: 50px;
}
</style>