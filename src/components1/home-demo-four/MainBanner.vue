<template>
    <div class="banner-wrapper">
        <div class="container-fluid">
            <div class="row align-items-center">
                <div class="col-lg-6 col-md-12">
                    <div class="banner-wrapper-content">
                        <h1>أهلا وسهلا بك في منصة تعميد</h1>
                        <p>أول منصة متكاملة في عالم التشييد والبناء في المملكة العربية السعودية
                            تقدم حلول لجميع المنشآةو الحصول على المشاريع الخاصة بشكل سريع وسهل
                        </p>
                        <router-link to="/contact" class="btn btn-primary">
                               سجل الآن
                        </router-link>
                    </div>
                </div>

                <div class="col-lg-6 col-md-12">
                    <div class="banner-wrapper-image">
                        <img src="../../assets/images/tt.png" alt="image">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainBanner'
    }
</script>