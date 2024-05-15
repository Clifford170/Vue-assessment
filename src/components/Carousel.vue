<script setup>

    import { Swiper, SwiperSlide } from 'swiper/vue'
    import { Navigation,Pagination } from 'swiper/modules'
    import "swiper/css"
    import 'swiper/css/navigation'
    import 'swiper/css/pagination'
    import { updateStyle as __vite__updateStyle, removeStyle as __vite__removeStyle } from "/@vite/client"
    const slides = [
        {
            icon: "/src/assets/Exprerian/CompuloanLogo.png",
            image: "/src/assets/Exprerian/Carousal1.png",
            description: "The PurQ service provides academic enrolment or qualification verification on an individual, in respect of an extensive list of participating academic institutions."
        },
        {
            icon: "/src/assets/Exprerian/ColumbusLogo.png",
            image: "/src/assets/Exprerian/Carousal1 – 1.png",
            description: "Columbus provides highly effective search functionalities that enable you to efficiently search for missing debtors, obtain their contact information, and establish their whereabouts..."
        },
        {
            icon: "/src/assets/Exprerian/CodixLogo.png",
            image: "/src/assets/Exprerian/Carousal1 – 2.png",
            description: "This service allows a 3rd party to retrieve a PDF Consumer Credit Report based on a previous enquiry or by doing a full enquiry"
        },
        {
            icon: "/src/assets/Exprerian/XceleratorLogo.png",
            image: "/src/assets/Exprerian/Carousal1 – 3.png",
            description: "The Employment Confidence Index (ECI) is a tool used to indicate the most probable employer listed on Experian’s credit bureau."
        },
        {
            icon: "/src/assets/Exprerian/AASLogo.png",
            image: "/src/assets/Exprerian/Carousal1 – 4.png",
            description: "The Identity Verification Service provides real-time verification on the identity of a consumer.."
        },
        {
            icon: "/src/assets/Exprerian/IncomePredictorLogo.png",
            image: "/src/assets/Exprerian/Carousal1 – 5.png",
            description: "Experian's Know Your Customer service, provides subscribers with consumer identity verification, contact numbers, address and employment information."
        }
    ]
</script>
<template>
  <div class="container-fluid carousel">
  <div class="row">
    <div class="col-12 power">Powerful Data <span> <img src="/src/assets/Exprerian/DrivenWording.png" alt=""></span> Tools to Help</div>
    <div class="col-12 thrive"> Your Thrive</div>
    <div class="col-12 ourData">Our data-driven products can significantly reduce costs while increasing your overall profit margins</div>
  </div>



  <div class="row shiftDown">
    <div class="col-1  center">
      <i class="bi bi-chevron-compact-left left button-prev "
       :click="() => btns.slidePrev()" style ="font-size: 3rem;  color: white" ></i>
    </div>
    <div class="col-10">
      <Swiper :slides-per-view="3"
       :modules="[Navigation]" 
       :navigation="{nextEl: '.button-next', prevEl: '.button-prev'}"
       :loop="true"
       > 
       <SwiperSlide v-for="slide in slides" :key="slide">
         <div class="row">
          <div class="slide-container">
             <div class="slide-content">
                 <div class="card">
                   <span class="img"><img :src="slide.icon" ></span>
                   <div class="image-content">
                     <span class="overlay">
                       <div class="card-image">
                         <img :src="slide.image" class="image-card">
                       </div>
                     </span>
                   </div>
                   <div class="card-content">
                     <p class="thePurq text-wrap">
                       {{ slide.description}}
                     </p>
                   </div>
                   <hr class="solid">
                   <button class="button">Enquire</button>
                 </div>
             </div>
          </div>
         </div>
       </SwiperSlide>
      </Swiper> 
        </div>
        <div class="col-1 center">
          <i class="bi bi-chevron-compact-right right button-next " 
          :click="() => btns.slideNext()" style ="font-size: 3rem;  color: white" ></i>
        </div>
  </div>
  </div>
</template>


<style>
.carousel{
    background-color: transparent radial-gradient(closest-side at 49% 49%, #5081C1 0%, #1D4F91 100%) 0% 0% no-repeat padding-box;
    background-image: url("/src/assets/Exprerian/BG3.png");
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    min-height: 1000px;
    opacity: 1;

}
.power{
      position: relative;
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
    top: 50px;
    text-align: center;
    margin-bottom: 30px;
}

.thrive{
    
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
    text-align: center;
}
.ourData{
    text-align: center;
    font: normal normal bold 19px/30px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
    opacity: 1;
}

 .card-image.image-card{
    height: 100%;
    width: 100%;
    object-fit: cover;
}
.card{
    display: grid; 
    border-radius: 10px;
    width: 300px;
    height: 150px;
 
}

.image-content,.card-content{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 10px 14px;
}

.thePurq{
    align-items: center;

} 
.image-content{
   row-gap: 5px;
}
.button{
    align-self: end;
    margin-bottom: 10px;
    margin-right: 10px;
    background: #FFFFFF 0% 0% no-repeat padding-box;
    border: 1px solid #E63888;
    color: #E63888;
    border-radius: 8px;
    height: 32px;
    width: 70px;
}
.img{
    display: flex;
    justify-content: center;
    width: 100%;
}
.slide-container{
    display: grid;
    position: relative;
    justify-content: center;
}
.center{
   align-content: center;
  
}
.left,.right{
    position: relative;
}
.shiftDown{
    position: relative;
    top: 85px;
}

</style>