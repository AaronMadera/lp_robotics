<template>
    <div>
        <div class="container-fluid">
            <b-carousel
            class="ml-xl-2"
            id="carousel" :interval="4000" controls indicators
            img-width="1024" img-height="480" style="text-shadow: 1px 1px 2px #333;"
            >
                <b-carousel-slide v-for="slide in slides"
                 :img-src="slide.img_url"
                >                
                <h1>{{slide.title}}</h1>
                <h4>{{slide.description}}</h4>
                </b-carousel-slide>
            </b-carousel>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Layout',
        data() {
            return {
                slides: [
                    {
                        img_url: 'https://www.crossco.com/wp-content/uploads/2019/07/Automated-Guided-Vehicles-Schaper-1024x480.png',
                        title: 'Applications',
                        description: 'Best robotics application in the market!'
                    },
                    {
                        img_url: 'https://wyolab.com/wp-content/uploads/2018/12/dji-mavic-2-pro-1024x480.jpg',
                        title: 'Drones',
                        description: 'Drone specialists, with computer vission.'
                    },
                    {
                        img_url: 'https://www.robotict.com/wp-content/uploads/2019/02/robotic-process-automation-1024x480.jpg',
                        title: 'Innovation',
                        description: 'Innovation is our best. We rule in the market applications.'
                    },
                    {
                        img_url: 'http://cgo-tech.pl/wp-content/uploads/2018/01/slide2-1024x480.jpg',
                        title: 'Quality',
                        description: 'Very customizable products and first quality.'
                    },
                ],
            };
        },
        methods: {
        }
    }
</script>

<style>
</style>