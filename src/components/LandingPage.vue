<script setup>
</script>
<template>
   <div class="container-fluid con">
       <div class="slides">
                <div class="row navbarRaw">
                    <div class="col">
                            <span class="portal">
                                <img src="/src/assets/Exprerian/ProductPortalLogo.png">
                        </span>
                    </div>
                    <div class="col left">
                        <span class="login" >
                            Login
                        </span>
                        <span >
                            <button class="getStarted">
                                Get Started  <i class="bi bi-arrow-up-right"></i>
                            </button>
                        </span>
                       </div>

                    <div class="row theRowBest">
                            <div class="col-12 theBest">
                                    The Best and most Trusted<span> <br> <img class="financeMove" src="/src/assets/Exprerian/FinancialWording.png"></span> Products
                            </div>
                    </div>  
                    <div class="row group">
                            <div class="col-12 applications">
                                <img class="applPic" src="/src/assets/Exprerian/Infographic1.png">
                            </div>
                    </div>
                </div>          
       </div>
   </div>
</template>

<style>
.con{
    position: relative;
    padding: 0px 0px;
}
.slides{
    background-color: transparent linear-gradient(207deg, #ECF0F6 0%, #D6E3F3 100%) 0% 0% no-repeat padding-box;
    background-image: url("/src/assets/Exprerian/BG1.png");
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
     position: relative;
     width: 100%;
    min-height: 700px;
   
   
    opacity: 1;
}
.portal{
    position: relative;
    left: 38px;
    height: 50px;
    width: 200px;
    display: block;
}
.left{

    display: flex;
    height: 50px;
    justify-content: end;
    flex-wrap: inherit;
   
}
.navbarRaw{
    position: relative;
    top:0px;
    height: 50px;
     display: block;
    

}

.login{
    position: relative;
    top: 16px;
    font: normal normal bold 16px/20px Roboto;
    letter-spacing: 0px;
    color: #313133;
    opacity: 1;
    height: 21px;
    width: 40px;
    right: 50px;
}

.getStarted{
    position: relative;
    top:6px;
    width: 141px;
    height: 44px;
    background: #AF1685 0% 0% no-repeat padding-box;
    border: 1px solid #AF1685;
    border-radius: 5px;
    opacity: 1;
    right: 42px;
    font: normal normal bold 16px/20px Roboto;
    letter-spacing: 0px;
    color: #FFFFFF;

}
.theRowBest{
    position: relative;
    top: 60px;
}

.theBest{
    text-align: center;
    height: 200px;
    font: normal normal bold 50px/100px Roboto;
    letter-spacing: 0px;
    color: #19468D;
}
.finance{
    position: absolute;
    top: 72px;
    display: flex;
    justify-content: center;
}
.financeMove{
    height: 75px;
}
.group{
    position:relative;
    height:350px ;
    top: 50px;
}
.applications{
    display: flex;
    justify-content: center;
    height:350px ;
    
}
.applPic{
    position: relative;
    top:30px;

}

</style>
