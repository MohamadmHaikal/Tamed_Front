<template>
 <div class="blog-area ptb-70 pt-0">
        <div class="container">
            <div class="section-title">
                <div class="row">
                    <div class="col-md-6">
                <h4>الصفقات و المزادات</h4>

                    </div>
                    <div class="col-md-6">
                <a href="/contact" >جميع الخدمات</a>

                    </div>
                </div>
                </div>

    <div class="feedback-slides">
        <carousel :autoplay="5000" :settings="settings" :wrap-around="true" :breakpoints="breakpoints">
            <slide v-for="slide in carouselItems" :key="slide.id">
                <div class="row">

                        <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            
                            <div class="blog-post-content">
                                <h3 style="display: contents;"> 
                                    <router-link to="/blog-details" >استشارات وتصمصم نماذج الأعمال</router-link>
                                </h3>

                                <p>تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية</p>
                                <router-link to="/blog-details" class="btn" style="background: #4c9da5;color: aliceblue;">بدء الخدمة</router-link>
                            </div>
                        </div>
                    </div>

                       <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            
                            <div class="blog-post-content">
                                <h3 style="display: contents;"> 
                                    <router-link to="/blog-details" > تحديد وتعريف التحديات</router-link>
                                </h3>

                                <p>تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية</p>
                                <router-link to="/blog-details" class="btn" style="background: #4c9da5;color: aliceblue;">بدء الخدمة</router-link>
                            </div>
                        </div>
                    </div>

                       <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            
                            <div class="blog-post-content">
                                <h3 style="display: contents;"> 
                                    <router-link to="/blog-details" > توليد الأفكار وإدارتها</router-link>
                                </h3>

                                <p>تتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكوميةتتيح خدمة تحديد و تعريف التحديات لمنسوبي الجهات الحكومية</p>
                                <router-link to="/blog-details" class="btn" style="background: #4c9da5;color: aliceblue;">بدء الخدمة</router-link>
                            </div>
                        </div>
                    </div>
              
                </div>

            </slide>

            <template #addons>
                <Navigation />
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

    import 'vue3-carousel/dist/carousel.css';

    export default defineComponent({
        name: 'Sectiondeals',
        components: {
            Carousel,
            Slide,
            Navigation,
        },
        data: () => ({
            carouselItems: [{
                    id: 1,
                    image: require('../../assets/images/blog/blog-1.jpg'),
                    name: 'John Lucy',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. ',
                },
                {
                    id: 2,
                    image: require('../../assets/images/blog/blog-2.jpg'),
                    name: 'John Smith',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. ',
                },
                {
                    id: 3,
                    image: require('../../assets/images/blog/blog-3.jpg'),
                    name: 'Ross Taylor',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis..',
                },
                {
                    id: 4,
                    image: require('../../assets/images/clients/client-4.jpg'),
                    name: 'James Anderson',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis..',
                },
                {
                    id: 5,
                    image: require('../../assets/images/clients/client-5.jpg'),
                    name: 'Steven Smith',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. ',
                },
            ],
            settings: {
                itemsToShow: 1,
                snapAlign: 'center',
            },
        }),
    })
</script>