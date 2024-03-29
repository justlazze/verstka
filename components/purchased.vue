<template>
    <div class="purchased">
        <div class="purchased__title">
          Статистика выкупленных товаров
        </div>
        <div class="purchased__months">
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              10
            </div>
            <div class="purchased__months-prog">
            <span style="height: 50%;">

            </span>
            </div>
            <div class="purchased__months-desc">
              Август
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              11
            </div>
            <div class="purchased__months-prog">
              <span style="height: 53%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Сентябрь
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              12
            </div>
            <div class="purchased__months-prog">
              <span style="height: 56%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Октябрь
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              13
            </div>
            <div class="purchased__months-prog">
              <span style="height: 59%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Ноябрь
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              14
            </div>
            <div class="purchased__months-prog">
              <span style="height: 62%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Декабрь
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              15
            </div>
            <div class="purchased__months-prog">
              <span style="height: 65%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Январь
            </div>
          </div>
          <div class="purchased__months-column">
            <div class="purchased__months-purch">
              16
            </div>
            <div class="purchased__months-prog">
              <span style="height: 68%;">
              
              </span>
            </div>
            <div class="purchased__months-desc">
              Февраль
            </div>
          </div>
        </div>
    </div>
</template>


<script>

</script>



<style>

.purchased__months-prog span {
background: #306098;
border-radius: 2px;
bottom: 0;
display: block;
left: 50%;
margin-left: -5px;
position: absolute;
width: 100%;
}

.purchased__months-prog {
flex: 1 1 auto;
margin: 8px 0;
opacity: .4;
position: relative;
width: 10px;
}

.purchased__months-column {
align-items: center;
color: #306098;
display: flex;
height: 92px;
flex-direction: column;
font-size: 10px;
font-weight: 400;
text-align: center;
}

.purchased__months {
display: flex;
justify-content: space-between;
}

.purchased__title {
font-size: 16px;
font-weight: 600;
color: white;
transition: .2s;
width: 100%;
margin-bottom: 16px;
}

.purchased  {
width: 388px;
height: 160px;
background: linear-gradient(#75A4DB, #72ADF3);
border-radius: 16px;
position: relative;
padding: 17px;

  
}
</style>