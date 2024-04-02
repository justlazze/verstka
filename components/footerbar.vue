<template>
    <div class="footer">
        <AppContainer>
        <div class="footer__nav">
            <div class="footer__nav-block">
                <div class="footer__nav-block-menu-logoandinfo">
                    <div class="footer__nav-block-menu-logoandinfo-logo">
                    <img src="/navbrandlogo.svg" alt="">
                    </div>
                    <div class="footer__nav-block-menu-logoandinfo-info">
                    Сервис по выкупу и доставки из Китая
                    </div>
                    <div class="footer_nav-block-menu-logoandinfo-rights footerbtn">
                        <a href="">© 2024 ChinaSpace. Все права защищены.</a>
                    </div>
                </div>

            </div>
            <div class="footer__nav-block">
                <div class="footer__nav-block-menu">
                    Новый заказ
                </div>
                <div class="footer__nav-block-menu">
                    Главный экран
                </div>
                <div class="footer__nav-block-menu">
                    Мой профиль
                </div>
                <div class="footer__nav-block-menu">
                    Мои заказы
                </div>
                <div class="footer__nav-block-menu-docs footerbtn">
                    <a href="">Правовая документация</a>
                </div>

            </div>
            <div class="footer__nav-block">
                <div class="footer__nav-block-menu">
                    Избранные товары
                </div>
                <div class="footer__nav-block-menu">
                    Партнёрам
                </div>
                <div class="footer__nav-block-menu">
                    Акции
                </div>
                <div class="footer__nav-block-menu">
                    Помощь и обучение
                </div>
                <div class="footer__nav-block-menu-offer footerbtn">
                    <a href="">Публичная оферта</a>
                </div>
            </div>
            <div class="footer__nav-block3">
                <div class="footer__nav-block-menu">
                    8 (800) 333-52-62
                </div>
                <div class="footer__nav-block-menu">
                    hello@china-space.ru
                </div>
                <div class="footer__nav-block3-btns">
                    <div class="footer__nav-block3-btns-btn">
                        W/A
                    </div>
                    <div class="footer__nav-block3-btns-btn">
                        TG
                    </div>
                    <div class="footer__nav-block3-btns-btn">
                        VK
                    </div>
                </div>
                <div class="footer__nav-block3-policy footerbtn">
                    <a href="">Политика конфиденциальности</a>
                </div>
            </div>
        </div>
        
        </AppContainer>
    </div>
</template>



<style>

.footerbtn {
    cursor: pointer;
}

.footerbtn:after {
	display: block;
	left: 0;
	width: 0;
	height: 1px;
	background-color: #8e8e91;
	content: "";
	transition: width .2s ease-out; 
}

.footerbtn:hover:after,
.footerbtn:focus:after {
	width: 10px;
}

.footer__nav-block3-btns-btn:hover {
    background: #404040;
    
    color: white;
    transition: .2s;

}

.footer__nav-block3-btns-btn {
    cursor: pointer;
    transition: .2s;

}


.footer__nav-block-menu-docs {
    font-size: 12px;
    color: #7F8086;
    margin-top: 56px;
}

.footer_nav-block-menu-logoandinfo-rights {
    font-size: 12px;
    color: #7F8086;
    margin-top: 50px;
    padding: 16px;
    margin-left: -16px;
}

.footer__nav-block-menu-offer {
    font-size: 12px;
    color: #7F8086;
    margin-top: 56px;
}


.footer__nav-block3-policy {
    font-size: 12px;
    color: #7F8086;
    margin-top: 59px;
    font-weight: 400;
    margin-right: -50px;
}





.footer__nav-block3 {
    font-size: 16px;
    font-weight: 700;
    color: #2F2F2F;
}

.footer__nav-block-menu:after {
	display: block;
	left: 0;
	width: 0;
	height: 2px;
    border-radius: 1px;
	background-color: #404040;
	content: "";
	transition: width .2s ease-out; 
}

.footer__nav-block-menu:hover:after,
.footer__nav-block-menu:focus:after {
	width: 10px;
}

.footer__nav-block-menu {
    margin-bottom: 8px;
    cursor: pointer;
    transition: .2s ease-out;
}



.footer__nav-block-menu-logoandinfo-info {
    font-size: 14px;
    font-weight: 400;
    color: #7F8086;
    margin-top: 20px;
    margin-right: 115px;
}

.footer__nav-block {
    font-size: 14px;
    font-weight: 400;
    color: #404040;
}

.footer__nav-block-menu-logoandinfo {
    margin-right: 175px;
    
}

.footer__nav-block3-btns-btn {
    width: 47px;
    height: 36px;
    border: 1px solid #404040;
    border-radius: 8px;
    font-size: 12px;
    font-weight: 600;
    justify-content: center;
    align-items: center;
    display: flex;
    color: #404040;
}

.footer__nav-block3-btns {
    display: flex;
    justify-content: space-between;
    width: 163px;
}

.footer__nav {
    display: flex;
    flex: column;
    justify-content: space-between;
    margin-top: 16px;
}

.footer {
    height: 221px;
    background: #F8F8F8;
    position: relative;
    padding: 16px;
    display: flex;
    justify-content: space-between;
    margin-top: 90px;
}


</style>