<template>
    <div class="myorders">
        <div class="myorders__title">
            Мои заказы
        </div>
        <div class="myorders__info">
            <div class="myorder__info-numstat">
            <div class="myorders__info-numstat-number">
                Номер
            </div>
            <div class="myorders__info-numstat-status">
                Статус
            </div>
        </div>
        <div class="myorder__info-randelsum">
            <div class="myorders__info-ransum">
                Сумма выкупа
            </div>
            <div class="myorders__info-delsum">
                Сумма доставки
            </div>
        </div>
        </div>
        <div class="myorders__orders">
            <div class="myorders__orders-orders">
                <img class="imgstatus" src="/orderstatusmod.svg" alt="">
                <div class="myorders__orders-orders-num">
                    0000
                </div>
                <div class="myorders__orders-orders-status">
                    Модерация
                </div>
                <div class="myorders__orders-orders-ransum" style="color:#7F8086">
                    Скоро
                </div>
                <div class="myorders__orders-orders-delsum" style="color:#7F8086">
                    Скоро
                </div>
            </div>
            <div class="myorders__orders-orders">
                <img class="imgstatus" src="/orderstatusroad.svg" alt="">
                <div class="myorders__orders-orders-num">
                    0001
                </div>
                <div class="myorders__orders-orders-status">
                    В пути по Китаю
                </div>
                <div class="myorders__orders-orders-ransum">
                    51123₽
                </div>
                <div class="myorders__orders-orders-delsum">
                    22745₽
                </div>
            </div>
            <div class="myorders__orders-orders">
                <img class="imgstatus" src="/orderstatuswaitpayment.svg" alt="">
                <div class="myorders__orders-orders-num">
                    0002
                </div>
                <div class="myorders__orders-orders-status">
                    Ожидание оплаты товара
                </div>
                <div class="myorders__orders-orders-ransum">
                    203455 ₽ 
                </div>
                <div class="myorders__orders-orders-delsum">
                    140234₽
                </div>
            </div>
            <div class="myorders__orders-orders">
                <img class="imgstatus" src="/orderstatuscomplete.svg" alt="">
                <div class="myorders__orders-orders-num">
                    0003
                </div>
                <div class="myorders__orders-orders-status">
                    Выполнен
                </div>
                <div class="myorders__orders-orders-ransum">
                    143523₽
                </div>
                <div class="myorders__orders-orders-delsum">
                    122234₽
                </div>
            </div>
        </div>
        <div class="myorders__button">
            Весь список заказов
        </div>
    </div>
</template>









<style>

.imgstatus {
    left: 192px;
    position: relative;
    align-items: center;

}


.myorders__info-delsum {
    margin-left: 90px;
}

.myorders__info-numstat-number {
    margin-right: 146px;
}

.myorder__info-randelsum {
    display: flex;
}

.myorder__info-numstat {
    display: flex;
    justify-content: space-between;
}


.myorders__orders-orders-ransum {
    width: 238px;
    text-align: right;
    padding-right: 82px;
}

.myorders__orders-orders-status {
width: 193px;
margin-left: -9px;
}

.myorders__orders-orders-num {
    width: 195px;
    
}

.myorders__orders {
    margin-top: 8px;
}

.myorders__button:hover {
    background:none;
    transition: .2s ease-out;
    color: #404040;
    border: 1px solid #404040;
}

.myorders__button {
    height: 42px;
    margin-top: 27px;
    width: 184px;
    background: #404040;
    color: #FFFFFF;
    border-radius: 8px;
    align-items: center;
    display: flex;
    justify-content: center;
    font-size: 14px;
    font-weight: 700;
    transition: .2s ease-out;
    cursor: pointer;
}


.myorders__orders-orders-delsum {
    width: 15%;
    text-align: right;
}

.myorders__orders-orders-num {
    margin-left: 12px;
}

.myorders__orders-orders:hover {
    background: #e2e2e2;
    transition: .2s ease-out;
}
.myorders__orders-orders {
    background: #F2F2F2;
    width: 100%;
    display: flex;
    margin: 4px;
    height: 40px;
    border-radius: 8px;
    align-items: center;
    cursor: pointer;
    transition: .2s;
    font-size: 14px;
    font-weight: 400;
    text-align: left;
}

.myorders__orders-orders-status {
    font-weight: 600;
}

.myorders__info {
display: flex; 
justify-content: space-between;
margin-left: 12px;
margin-right: 12px;
margin-top: 19px;
}
.myorders__title {
    margin-bottom: 12px;
    font-size: 16px;
    font-weight: 600;
    color: #404040;
}

.myorders__info {
    font-size: 14px;
    font-weight: 400;
    color: #7F8086;
}



.myorders {
    width: 792px;
    height: 338px;
    background-color: #F8F8F8;
    border-radius: 16px;
    padding: 16px;
}
</style>





