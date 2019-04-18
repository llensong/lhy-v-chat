<template>
    <div class="lbt">
        <Carousel autoplay v-model="value2" loop>
            <CarouselItem v-for="item in listArr">
                <div class="demo-carousel"><img :src="item" alt=""></div>
            </CarouselItem>
            <!-- <CarouselItem>
                <div class="demo-carousel"><img src="../assets/23.jpg" alt=""></div>
            </CarouselItem>
            <CarouselItem>
                <div class="demo-carousel"><img src="../assets/24.jpg" alt=""></div>
            </CarouselItem>
            <CarouselItem>
                <div class="demo-carousel"><img src="../assets/25.jpg" alt=""></div>
            </CarouselItem>
            <CarouselItem>
                <div class="demo-carousel"><img src="../assets/984.jpg" alt=""></div>
            </CarouselItem> -->
        </Carousel>
    </div>
</template>
<script>
export default {
     data () {
            return {
                value2: 0,
                listArr:[
                     require("../assets/23.jpg"),
                     require("../assets/24.jpg"),
                     require("../assets/25.jpg"),
                     require("../assets/984.jpg"),
                     require("../assets/21.jpg"),
                ]
            }
        },
    methods:{
        lbt(){
           
        }
    }
}
</script>
<style >
    .lbt{
        width: 79%;
        height: 450px;
        margin: auto;
    }
</style>