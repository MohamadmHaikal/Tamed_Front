<template>
 <div class="blog-area ptb-70 pt-0">
        <div class="container">
            <div class="section-title">
                <div class="row">
                    <div class="col-md-6">
                <h4>أحدث المشاريع</h4>

                    </div>
                    <div class="col-md-6">
                <a href="/contact" > عرض الجميع </a>

                    </div>
                </div>
                </div>
    <div class="feedback-slides">
        <carousel :autoplay="5000000" :settings="settings" :wrap-around="true" :breakpoints="breakpoints">
            <slide v-for="slide in carouselItems" :key="slide.id">
                <div class="row">
                    <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            <div class="blog-image">
                                <router-link to="/blog-details">
                                    <img :src="slide.image" alt="image">
                                </router-link>

                                <div class="date">
                                    <i class="far fa-calendar-alt"></i> September 19, 2019
                                </div>
                            </div>

                            <div class="blog-post-content">
                                <h3>
                                    <router-link to="/blog-details">{{slide.name}}</router-link>
                                </h3>

                                <!-- <span>By <a href="#">{{slide.position}}</a></span> -->

                                <!-- <p>{{slide.description}}</p> -->
                                <!-- <router-link to="/blog-details" class="read-more-btn">Read More <i
                                        class="fas fa-arrow-right"></i></router-link> -->
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            <div class="blog-image">
                                <router-link to="/blog-details">
                                    <img :src="slide.image" alt="image">
                                </router-link>

                                <div class="date">
                                    <i class="far fa-calendar-alt"></i> September 19, 2019
                                </div>
                            </div>

                            <div class="blog-post-content">
                                <h3>
                                    <router-link to="/blog-details">{{slide.name}}</router-link>
                                </h3>

                                <!-- <span>By <a href="#">{{slide.position}}</a></span> -->

                                <!-- <p>{{slide.description}}</p> -->
                                <!-- <router-link to="/blog-details" class="read-more-btn">Read More <i
                                        class="fas fa-arrow-right"></i></router-link> -->
                            </div>
                        </div>
                    </div>

                    <div class="col-lg-4 col-md-6 offset-lg-0 offset-md-3">
                        <div class="single-blog-post">
                            <div class="blog-image">
                                <router-link to="/blog-details">
                                    <img :src="slide.image" alt="image">
                                </router-link>

                                <div class="date">
                                    <i class="far fa-calendar-alt"></i> September 19, 2019
                                </div>
                            </div>

                            <div class="blog-post-content">
                                <h3>
                                    <router-link to="/blog-details">{{slide.name}}</router-link>
                                </h3>

                                <!-- <span>By <a href="#">{{slide.position}}</a></span> -->

                                <!-- <p>{{slide.description}}</p> -->
                                <!-- <router-link to="/blog-details" class="read-more-btn">Read More <i
                                        class="fas fa-arrow-right"></i></router-link> -->
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
        name: 'SectionProject',
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
                    image: require('../../assets/images/blog/blog-3.jpg'),
                    name: 'James Anderson',
                    position: 'Web Developer',
                    description: 'Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis..',
                },
                {
                    id: 5,
                    image: require('../../assets/images/blog/blog-2.jpg'),
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