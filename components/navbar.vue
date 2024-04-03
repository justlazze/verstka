<template>
    <div class="navbar">
        <AppContainer>
                    <div class="brand-logo"> 
                <a href="/">
                    <img src="navbrandlogo.svg" alt="На главную">
                </a>

            </div>
            <div class="nav-items">
                <ul class="nav-item">
                    <li class="nav-link">
                        

                        
                        <a href="#" class="navli">
                            <img src="/navneworderico.svg" alt="" class="navicons">
                            Новый заказ</a>
                    </li>
                    <li class="nav-link">
                        

                        <a href="orders" class="navli">
                            <img src="/navordersico.svg" alt="" class="navicons">
                            Заказы</a>
                    </li>
                    <li class="nav-link notifybutton"  @click="toggle" v-click-outside="hide">
                        

                        <a :class="{'active' : isShow}" href="#" class="navli">
                            <img src="/navnotifico.svg" alt="" class="navicons">
                            Уведомления</a>
                            <div class="notifylayer" :class="{'opened': isShow}" @click.stop>
                                <div class="title">
                                    Уведомления
                                </div>
                                <div class="notifylayer__btns">
                                    <div class="notifylayer__btns-btn">
                                        Все
                                    </div>
                                    <div class="notifylayer__btns-btn">
                                        Сообщения
                                    </div>
                                    <div class="notifylayer__btns-btn">
                                        Заказы
                                    </div>
                                    <div class="notifylayer__btns-btn">
                                        Акции
                                    </div>
                                </div>
                                <div class="notifylayer__orders">
                                    <div class="notifylayer__orders-order">
                                        <div class="notifylayer__orders-order-checkbox">
                                       <input type="checkbox">
                                    </div>
                                       <div class="notifylayer__orders-order-line"></div>
                                        <div class="notifylayer__orders-order-info">
                                            <div class="notifylayer__orders-order-info-title">
                                                Изменения в статусе заказа X-0123-010
                                            </div>
                                            <div class="notifylayer__orders-order-info-date">
                                                04.08.2023
                                            </div>
                                            <div class="notifylayer__orders-order-info-btn">
                                                Перейти
                                        </div>
                                        </div>
                                        <svg width="8" height="8" viewBox="0 0 8 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path d="M0.666016 0.666016L7.33268 7.33268M0.666016 7.33268L7.33268 0.666016" stroke="#D4D4D4" stroke-linecap="round" stroke-linejoin="round"/>
                                        </svg>

                                    </div>
                                    <div class="notifylayer__orders-order">
                                        <div class="notifylayer__orders-order-checkbox">
                                        <input type="checkbox">
                                    </div>
                                       <div class="notifylayer__orders-order-line"></div>
                                       <div class="notifylayer__orders-order-info">
                                        <div class="notifylayer__orders-order-info-title">
                                            Акция: поделись промокодом и получили скидку 10% на второй заказ
                                        </div>
                                        <div class="notifylayer__orders-order-info-date">
                                            24.07.2023
                                            </div>
                                        <div class="notifylayer__orders-order-info-btn">
                                            Перейти
                                        </div>
                                        </div>
                                        <svg width="8" height="8" viewBox="0 0 8 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path d="M0.666016 0.666016L7.33268 7.33268M0.666016 7.33268L7.33268 0.666016" stroke="#D4D4D4" stroke-linecap="round" stroke-linejoin="round"/>
                                        </svg>

                                    </div>
                                    <div class="notifylayer__orders-order">
                                        <div class="notifylayer__orders-order-checkbox">
                                        <input type="checkbox">
                                        </div>
                                       <div class="notifylayer__orders-order-line"></div>
                                       <div class="notifylayer__orders-order-info">
                                        <div class="notifylayer__orders-order-info-title">
                                            Обновление платформы: узнайте как мы изменили интерфейс и какие функции теперь доступны
                                            </div>
                                            <div class="notifylayer__orders-order-info-date">
                                                10.07.2023
                                            </div>
                                            <div class="notifylayer__orders-order-info-btn">
                                                Перейти
                                        </div>
                                        </div>
                                        <svg width="8" height="8" viewBox="0 0 8 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path d="M0.666016 0.666016L7.33268 7.33268M0.666016 7.33268L7.33268 0.666016" stroke="#D4D4D4" stroke-linecap="round" stroke-linejoin="round"/>
                                        </svg>

                                    </div>
                                </div>
                                <div class="notifylayer__footer">
                                    <div class="notifylayer__footer-btns">
                                        <div class="notifylayer__footer-btns-btn">
                                            Отметить все как прочитанное
                                        </div>
                                        <div class="notifylayer__footer-btns-btn">
                                            Очистить все
                                        </div>
                                    </div>
                                </div>
                            </div>
                    </li>
                    <li class="nav-link">
                        
                        <a href="#" class="navli">
                            <img src="/navhelpico.svg" alt="" class="navicons">
                            Помощь</a>
                        
                    </li>
                    
                </ul>
                <HeaderProfile />
            </div>
            </AppContainer>
        </div>
    
    
</template>

<script>
import vClickOutside from 'v-click-outside'
import AppContainer from "~/components/app-container.vue"
export default {
    components: {
        AppContainer},
    props: {
        
    },
    directives: {
      clickOutside: vClickOutside.directive
    },
    data() {
        return {
            isShow: false,
        }
    },
    methods: {
        toggle() {
            this.isShow = !this.isShow
        },
        show() {
            this.isShow = true
        },
        hide() {
            this.isShow = false
        },
        
    }
    

}
</script>

<style lang="scss" scoped>




.notifylayer {
    position: absolute;
    top: 40px;
    left: 0;
    background: #F8F8F8;
    border-radius: 16px;
    z-index: 10;
    display: none;
    width: 390%;
    cursor: default;
    transition: .2s ease-out;
    padding: 24px;
    &.opened {
        display: block;
        height: auto;
        cursor: default;
        filter: drop-shadow(0px 1px 5.7px rgba(69, 69, 69, 0.2));
    }


    &__footer {
        background: radial-gradient(126.26% 557.1% at 7.88% 95.89%, #AE72B3 0%, #A17ACC 20.17%, #837DCC 62.2%, #697EC8 100%);
        border-radius: 0px 0px 16px 16px;
        margin-right: -24px;
        margin-left: -24px;
        margin-bottom: -24px;
        margin-top: 24px;

        &-btns {
            display: flex;
            justify-content: space-between;
            padding: 24px;
            &-btn {
                color: #FFFFFF;
                font-size: 12px;
                font-weight: 600;
            }
        }
    }

    &__orders {
        &-order {
            display: flex;
            margin-top: 8px;
            padding-bottom: 9px;
            border-bottom: #F2F2F2 solid 1px;
            position: relative;
            &-line {
                height: auto;
                width: 2px;
                background: linear-gradient(to top, #86DE76, #6EAD63);
                margin-right: 12px;
                margin-left: 12px;
                border-radius: 1px;
                
            }
            & svg {
                position: absolute;
                top: 0px;
                right: 0px;
                cursor: pointer;
                & path {
                    transition: .2s ease;
                }
                &:hover path{
                    stroke: #404040;
                    transition: .2s ease;
                }
            }
            &-info {
                margin-right: 50px;
                &-title {
                    color: #404040;
                    font-size: 12px;
                    font-weight: 600;
                    line-height: 15.6px;
                }
                &-date {
                    color: #7F8086;
                    font-size: 10px;
                    font-weight: 400;
                    margin-top: 8px;
                }
                &-btn {
                    color: #404040;
                    font-size: 12px;
                    font-weight: 600;
                    margin-top: 8px;
                }
            }
        }
    }

    &__title {
        font-size: 14px;
        font-weight: 600;
    }

    &__btns {
        display: flex;
        margin-top: 24px;
        margin-bottom: 16px;
        &-btn {
            padding: 8px 16px 8px 16px;
            border: 1px solid #D4D4D4;
            border-radius: 8px;
            font-size: 12px;
            font-weight: 600;
            margin-right: 4px;
            cursor: pointer;
            transition: .2s ease;
            &:hover {
                background: #404040;
                border: 1px solid #404040;
                color: #FBFBFB;
                transition: .2s ease;
            }

        }
    }

}

.notifybutton {
    position: relative;
}

.navbar {
    display: flex;
    justify-content: center;
    margin-top: 20px;
    margin-bottom: 60px;
}

.navbar .app-container {
    margin: 0 auto;
    display: flex;
    height: 46px;

    align-items: center;
    justify-content: space-between;
}

.brand-logo {
    width: 166px;
    align-content: space-between;
    display: flex;
    align-items: center;
    margin-top: 2px;
    transition: .2s ease;
}

.brand-logo:hover {
    cursor: pointer;
    filter: brightness(1.1);
    transition: .2s ease;
}

.nav-items {
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

.nav-link.profile {
    display: inline-block;
    margin-right: 0px;
}

.nav-link {
    display: inline-block;
    margin-right: 32px;
    line-height: 1  ;
    margin-top: 1px;
    transition: .2s ease-out;


}

.nav-link:hover .navicons {
    transform: scale(1.1);
    transition: .3s ease;
}

.nav-item {
    text-decoration: none;
}

.nav-link a {
    border-radius: 8px;
    color: var(--color-black);
    cursor: pointer;
    font-size: 14px;
    font-weight: 600;
    padding: 8px 6px;
    text-decoration: none;
    transition: .3s ease;
    white-space: nowrap;
}

.navicons {
    max-height: 24px;
    max-width: 24px;
    margin: 0;
    vertical-align: middle;
    transition: .3s ease;
    margin-top: -3px;
    
}

.nav-link:hover a {
    background: #F2F2F2;
}

.nav-link a.active{
    background: #F2F2F2;
}

.nav-link .active .navicons {
    transform: scale(1.1);
    transition: .3s ease;
}
</style>