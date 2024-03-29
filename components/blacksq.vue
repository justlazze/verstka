
<template>
    
    <div class="blacksquare">
        
            

        
        
        
        <div class="blacksquare__minsq">
            
                <img v-if="icon === 'plus'" src="/cardneworderico.svg" alt="">
                <img v-else-if="icon === 'packet'" src="/favouritescardico.svg" alt="">
                <img v-else-if="icon === 'box'" src="/myorderscardico.svg" alt="">
                <img v-else-if="icon === 'help'" src="/helpcardico.svg" alt="">


            
        </div>
        
        <div class="blacksquare__row">
            <svg width="8" height="8" viewBox="0 0 8 8" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.91767 6.23137C6.86839 6.23139 6.81959 6.22171 6.77406 6.20286C6.72852 6.18401 6.68715 6.15638 6.6523 6.12153C6.61745 6.08669 6.58982 6.04531 6.57097 5.99978C6.55212 5.95424 6.54244 5.90544 6.54247 5.85616L6.5428 1.98839L1.34921 7.18198C1.27888 7.25231 1.1835 7.29182 1.08404 7.29182C0.984588 7.29182 0.889205 7.25231 0.818878 7.18198C0.748552 7.11166 0.709044 7.01627 0.709043 6.91682C0.709043 6.81736 0.748553 6.72198 0.818878 6.65165L6.01247 1.45806L2.1447 1.4584C2.04519 1.4584 1.94976 1.41886 1.87939 1.3485C1.80903 1.27813 1.76949 1.1827 1.76949 1.08319C1.76949 0.983676 1.80903 0.88824 1.87939 0.817875C1.94976 0.747509 2.04519 0.707979 2.1447 0.707979L6.91767 0.707978C6.96695 0.707951 7.01576 0.717638 7.06129 0.736484C7.10683 0.75533 7.1482 0.782967 7.18305 0.817813C7.21789 0.85266 7.24553 0.894034 7.26438 0.939569C7.28322 0.985103 7.29291 1.03391 7.29288 1.08319L7.29288 5.85616C7.29291 5.90544 7.28322 5.95424 7.26438 5.99978C7.24553 6.04531 7.21789 6.08668 7.18305 6.12153C7.1482 6.15638 7.10683 6.18402 7.06129 6.20286C7.01576 6.22171 6.96696 6.23139 6.91767 6.23137Z" fill="white"/>
</svg>

        </div>
        <div class="blacksquare__title">
            {{ title }}
        </div>
        <div class="blacksquare__text">
            {{ text }}
        </div>
  </div>
    
</template>



<script>
export default {
    props: {
        icon: {
            type: String, 
            default: ""
        },
        title: {
            type: String,
            default: ""
        },
        text: {
            type: String,
            default: ""
        }
    }
}
</script>



<style>


.blacksquare__text {
    color: #CDCDCD;
    font-size: 12px;
    font-weight: 400; 
}

.blacksquare__title {
    color: white;
    font-size: 14px;
    font-weight: 700;
}



.blacksquare {
    width: 184px;
    height: 158px;
    border-radius: 16px;
    background: #404040 url("/svgblackbacksq.svg") center center no-repeat;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    position: relative;
    cursor: pointer;
    transition: .2s ease-out;
    padding: 16px;
   
}

.blacksquare__minsq {
    width: 48px;
    height: 48px;
    background-color: #4D4D4D;
    display: flex;


    border-radius: 8px;


    align-items: center;
    justify-content: center;
    transition: .2s ease-out;

}

.blacksquare__minsq img {
    display: block;
    
}

.blacksquare__row {
    margin-top: 16px;
    margin-right: 13px;
    display: flex;
    width: 12px;
    height: 12px;
    position: absolute;
    right: 0px;
    top: 0px;
    transition: .2s ease-out;

    
}

.blacksquare:hover .blacksquare__row {
    
    transform: translateX(3px) translateY(-3px);
    

   
}


.blacksquare:hover {
    cursor: pointer;
    background-color: #464646;
    transition: .2s ease-out;
    
}



.blacksquare:hover .blacksquare__minsq {
    transform: scale(0.9);
    transition: .2s ease-out;
}




</style>