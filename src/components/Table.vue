<script setup>
import Infomation from '../../src/Information.json'

const dataTable = Infomation;
 </script>

<template>
<div class="container-fluid containerr">
 <div class="row">
     <div class="row">
         <div class="col-12 innovated">Innovated Products That Gives You all <br>
              The <span><img src="/src/assets/Exprerian/InformationWording – 1.png" alt=""></span> You Need</div>
     </div>
 </div>
 <div class="col-12 shiftTable">
         <div class="home" >
             <div class="container table">
                 <div class="row rowTable">
                     <div class="col-md-2 headings">Product</div>
                     <div class="col-md-2 headings">Feature #1</div>
                     <div class="col-md-2 headings">Feature #2</div>
                     <div class="col-md-2 headings">Feature #3</div>
                     <div class="col-md-2 headings">Feature #4</div>
                     <div class="col-md-2 headings">Feature #5</div>
                 </div>
                 <div class="row rowTable" v-for="data in dataTable" :key="data">
                     <div class="col-md-2 fields"> {{data.product}}</div>
                     <div class="col-md-2 fields"><i v-if="data.feature1 === 'x'" class="bi bi-check-circle-fill" style="color: green;background-color:#F0E9F1;"></i></div>
                     <div class="col-md-2 fields"><i v-if="data.feature2 === 'x'" class="bi bi-check-circle-fill" style="color: green;background-color:#F0E9F1;"></i></div>
                     <div class="col-md-2 fields"><i v-if="data.feature3 === 'x'" class="bi bi-check-circle-fill" style="color: green;background-color:#F0E9F1;"></i></div>
                     <div class="col-md-2 fields"><i v-if="data.feature4 === 'x'" class="bi bi-check-circle-fill" style="color: green;background-color:#F0E9F1;"></i></div>
                     <div class="col-md-2 fields"><i v-if="data.feature5 === 'x'" class="bi bi-check-circle-fill" style="color: green;background-color:#F0E9F1;"></i></div>
                  </div>
                 </div>
</div>
     </div>
</div>
</template>


<style>
.containerr{
     width: 1920px;
     min-height: 2000px;
     background-color: #FFFFFF 0% 0% no-repeat padding-box;
     opacity: 1;
 }
 .innovated{
         top: 0px;
         left: 39px;
         width: 1201px;
         height: 92px;
         /* UI Properties */
         text-align: center;
         font: normal normal bold 50px/100px Roboto;
         letter-spacing: 0px;
         color: #1D4F91;
  }

  .home {
     position: relative;
     max-width: 850px;
     color: #2c3e50;
     display: flex;
     background-color: #F0E9F1 0% 0% no-repeat padding-box;
     align-self: center;
     border-radius: 12px;
     margin-right: 15rem;
    
  }
     .rowTable {
         border: 1px solid #6D2077;
     }
     .headings{
         display: flex;
         padding-top: 10px;
         padding-bottom: 10px;
         border-right: 1px solid #6D2077;
         background: #F0E9F1 0% 0% no-repeat padding-box;

     }
     .fields {
         display: flex;
         padding-top: 10px;
         padding-bottom: 10px;
         border-right: 1px solid #6D2077;
         justify-content: center;
         background: #F0E9F1 0% 0% no-repeat padding-box;      
         font: normal normal bold 12px/28px Roboto;
         letter-spacing: 0px;
         color: #333333;
         opacity: 1;
    
     }

     .headings {
         background-color: #f1f1f1;
     }        
     .shiftTable{
         position: relative;
         top: 150px;
         margin-left: 20rem;

     }
     .start{
         display: flex;
         justify-content: start;
     }

</style>