<template>
    
    <div class="greensquare">
        <div class="greensquare__valueusers">
            {{ valueusers }}
        </div>
        <div class="orangesquare__title">
            {{ title }}
        </div>
        <div class="orangesquare__text">
            {{ text }}
        </div>
        
  </div>
    
</template>

<script>
    export default {
        props: {
            title: {
                type: String,
                default: ""
            },
            text: {
                type: String,
                default: ""
            },
            valueusers: {
                type: String,
                default: ""
            }
        }
    }
</script>



<style>
.greensquare__text {
    color: #FFFFFF;
    font-size: 12px;
    font-weight: 400; 
}

.greensquare__title {
    color: white;
    font-size: 14px;
    font-weight: 600;
}


.greensquare__valueusers{
    font-size: 20px;
    font-weight: 600;
    color: white;
    transition: .2s;
    width: 100%;
}





.greensquare{
    width: 184px;
    height: 158px;
    border-radius: 16px;
    background: linear-gradient(#599C4B, #8FC466);
    display: flex;
    position: relative;
    margin: 10px;
    background: url(/greensq.png) center center no-repeat;







    flex-direction: column;
    justify-content: space-between;

    transition: .2s ease-out;
    padding: 16px;
    
   
}

</style>