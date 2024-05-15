<script setup>
  
</script>
<template>
  <div class="container-fluid contain">
    <div class="row m">
        <div class="col-4">
            <img class="image" src="/src/assets/Exprerian/Infographic2.png">
        </div>
        <div class="col-8 shiftdown">
            <div class="row financial">
                <div class="col-12">
                    Financial <img class="InsightsWording" src="/src/assets/Exprerian/InsightsWording.png">in the <br>Palm of Your Hands
                </div>
            </div>
            <div class="row">
                <div class="col driveIntelligent">
                    Drive intelligent decisions, new product innovation and better targeting through insight <br>
                    and technology. Helping to deliver a frictionless digital customer experience.
                </div>
            </div>
        </div>
    </div>
  </div>
</template>


<style>
.contain{
    background-color: transparent url('img/banner-hero-purple-squircles-background-m.png') 0% 0% no-repeat padding-box;
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    opacity: 1;
    background-image: url("/src/assets/Exprerian/BG2.png");
    min-height: 450px;
}
.image{
    top: 50px;
    position: relative;
    height: 400px;
    left: 100px;
    width: 100%;
}
.financial{
    text-align: left;
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
}
.inThe{
    text-align: left;
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
}
.shiftdown{
    position: relative;
    top: 100px;
}
.palm{
    position:absolute;
    height: 86px;
    text-align: left;
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
    top: 80px;

}
.InsightsWording{
    height: 80px;
}
.driveIntelligent{
    text-align: left;
    font: normal normal normal 16px/30px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;
    opacity: 1;
    top: 0px;
    height: 70px;

}
</style>