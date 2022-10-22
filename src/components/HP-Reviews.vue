<template>
    <div class="reviews-container">
        <h1 class="reviews-title">Read our Reviews</h1>
        <swiper
        :modules="modules"
        :slides-per-view="3"
        :space-between="50"
        navigation
        :pagination="{ clickable: true }"
        :scrollbar="{ draggable: true }"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
    >
    
        <swiper-slide v-for="(review) in reviews" :key="review" :style="'background-color=white'">
        
            <div class="review-body" >
                <p><b>{{review.label}}</b></p>  
                <p >{{review.value}}</p>
                <div class = "rating">
                    <fa icon="fa-solid fa-star"></fa>
                    <fa icon="fa-solid fa-star"></fa>
                    <fa icon="fa-solid fa-star"></fa>
                    <fa icon="fa-solid fa-star"></fa>
                    <fa icon="fa-solid fa-star"></fa>
                </div>
    
            </div>      
        
    
    
    
    
    
        </swiper-slide>
    
    </swiper>       
    </div>
    
    </template>
    
    
    <style>
    .reviews-container{
        background-color: #023047;
        text-align: center;
    }
    
    .reviews-title{
        color: white;
        font-weight: bold;
        padding-top: 50px;
        text-align: center;
    }
    
    .swiper{
        display: flex;
        background-color: #023047;
        /* margin-top: 20px; */
        width: 100%;
        justify-content: space-between;
        height: 500px;
    
        box-shadow: rgba(0, 0, 0, 0.25) 0px 14px 28px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
    }
    
    
    
    .review-body{
        display: flex;
        flex-direction: column;
        /* background-color: #B758F8; */
        background: white;
        margin: 50px;
        padding: 10px;
        width: 500px;
        border-radius: 10px;
        height: 250px;
        margin-top: 60px;
        box-shadow: rgba(0, 0, 0, 0.25) 0px 14px 28px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
    }
    
    .rating{
        padding-bottom: 10px;
    }
    
    
    </style>
    
    <script>
    // import Swiper core and required modules
    import { Navigation, Pagination, Scrollbar, A11y } from 'swiper';
    
    // Import Swiper Vue.js components
    import { Swiper, SwiperSlide } from 'swiper/vue';
    
    // Import Swiper styles
    import 'swiper/css';
    import 'swiper/css/navigation';
    import 'swiper/css/pagination';
    import 'swiper/css/scrollbar';
    
    // Import Swiper styles
    export default {
        components: {
        Swiper,
        SwiperSlide,
        },
    
        data() {
            return {
                reviews: [
                    {value: '"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae a repellat aspernatur similique, perferendis eligendi placeat, laborum saepe odit magni doloremque vero dolorum totam deleniti ab ullam tempore voluptatum fugit"', label: "Mo Smith"},
                    
                    {value: '"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae a repellat aspernatur similique, perferendis eligendi placeat, laborum saepe odit magni doloremque vero dolorum totam deleniti ab ullam tempore voluptatum fugit"', label: "Walker Smith", color:"#FEC400" }, 
                    
                    {value: '"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae a repellat aspernatur similique, perferendis eligendi placeat, laborum saepe odit magni doloremque vero dolorum totam deleniti ab ullam tempore voluptatum fugit"', label: "Mo Smith"},
                    
                    {value: '"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae a repellat aspernatur similique, perferendis eligendi placeat, laborum saepe odit magni doloremque vero dolorum totam deleniti ab ullam tempore voluptatum fugit"', label: "Walker Smith", color:"#FEC400" }, 
    
                    
                    ],
            };
        },
        setup() {
        const onSwiper = (swiper) => {
            console.log(swiper);
        };
        const onSlideChange = () => {
            console.log('slide change');
        };
        return {
            onSwiper,
            onSlideChange,
            modules: [Navigation, Pagination, Scrollbar, A11y],
        };
        },
    };
    </script>