<template>
    <div class="blog-area ptb-70 pt-0">
        <div class="container">
            <div class="section-title" >
                <div class="row">
                    <div class="col-md-6">
                        <h4>الصفقات و المزادات</h4>

                    </div>

                    <!-- <div class="col-md-6">
                <a href="/contact" class="button">جميع الخدمات</a>

                    </div> -->
                </div>
            </div>


            <div class="feedback-slides">
                <carousel :autoplay="500000" :settings="settings" :wrap-around="true" :breakpoints="breakpoints">
                    <slide v-for="slide in carouselItems" :key="slide.id">

                        <div class="single-deals-post">

                            <div class="deals-post-content">
                                <div class="row section-title">
                                    <span >شركة فرسان</span>
                                    <h5 class="titleDEals">
                                        <router-link to="/blog-details">{{slide.title}}</router-link>
                                        <i class="fas fa-angle-left	" ></i>
                                    </h5>

                                    <p class="desc">{{ slide.description }}</p>


                                </div>
                                <div class="row" >
                                    
                                    <span>تنتهي الصفقة في</span>
                                        <div >
                                            <Countdown deadline="2023-12-25 00:00:00" :showLabels="false"
                                          mainFlipBackgroundColor="#d7a358"
                                          secondFlipBackgroundColor="#d7a358"
                                          countdownSize="1.1rem"
                                            mainColor="#ffff"/>

                                        </div>
                                </div>

                                <div class="row pt">
                                    <div class="col-md-6">
                                       

                                        <router-link to="/blog-details" class="btn link"
                                          >{{ slide.button }}
                                        </router-link>
                                    </div>
                                    <div class="col-md-6 pt-3">
                                        <h6 class="typeDeals">{{  slide.typeDeals }}</h6>
                                        <span >{{  slide.price }}</span>
                                    </div>

                                </div>

                            </div>
                        </div>

                    </slide>

                    <template #addons>
                        <!-- <Navigation /> -->
                    </template>
                </carousel>
            </div>
        </div>
    </div>


</template>

<script>
    import {
        defineComponent
    } from 'vue';
    import {
        Carousel,
        Slide,
        Navigation
    } from 'vue3-carousel';
    import {
        Countdown
    } from 'vue3-flip-countdown'

    import 'vue3-carousel/dist/carousel.css';

    export default defineComponent({
        name: 'Sectiondeals',
        components: {
            Countdown,
            Carousel,
            Slide,
            Navigation,
        },
        data: () => ({
            carouselItems: [{
                    id: 1,
                    title: 'استشارات و تصميم نماذج الأعمال',
                    typeDeals: 'صفقة بقيمة',
                    price: '500000 ريال',
                    button: 'شراء',
                    color:'#ebde46',
                    description: 'تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية',
                },
                {
                    id: 2,
                    title: 'شراء مواد حديد',
                    typeDeals: 'سعر المشاركة بالمزاد',
                     price: '500 ريال تأمين',
                    button: 'مشاركة بالمزاد',
                    description: 'تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية',
                },
                {
                    id: 3,
                    title: 'توليد الأفكار و إدارتها',
                    typeDeals: 'صفقة بقيمة',
                    price: '500000 ريال',
                    button: 'شراء',
                    description: 'تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية',
                },
                {
                    id: 4,
                        typeDeals: 'مزاد',
                    button: 'مشاركة بالمزاد',
                    description: 'تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية',
                },
                {
                    id: 5,
                        typeDeals: 'صفقة بقيمة',
                    price: '500000 ريال',
                    button: 'شراء',
                    description: 'تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية',
                },
            ],
            settings: {
                itemsToShow: 3,
                snapAlign: 'center',
            },
        }),
    })

</script>
