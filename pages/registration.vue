<template>
    <main>
        <AppContainer>
            <div class="layer">
                <div class="registration">
                    <div class="registration__title">
                        Регистрация
                    </div>
                    <div class="registration__form">
                        <div class="registration__form-title">
                            ФИО
                        </div>
                        <div class="input">
                            <input type="text" placeholder="Иванов Николай Иванович" required>
                        </div>
                        <div class="registration__form-title">
                            E-mail
                        </div>
                        <div class="input">
                            <input type="text" placeholder="name@email.com" required>
                        </div>
                        
                        <div class="registration__form-title">
                            Телефон
                        </div>
                        <div class="input">
                            <input type="text" placeholder="+7 (999) 999-99-99" required>
                        </div>
                        <div class="registration__form-title">
                            Пароль
                        </div>
                        <div class="input">
                            <input type="text" placeholder="Введите пароль" required>
                        </div>
                        <div class="input">
                            <input type="text" placeholder="Повторите пароль" required>
                        </div>
                    </div>
                    <div class="registration__policy">
                        <input type="checkbox" required/>
                        <span>Продолжая регистрацию я соглашаюсь с <a href="#">политикой конфиденциальности</a></span>
                    </div>
                    <button>Зарегистрироваться</button>
                    <div class="registration__alt">
                        <div class="registration__alt-title">
                            <span>Или</span>
                        </div>
                        <div class="registration__alt-btns">
                            <div class="registration__alt-btns-btn">
                                <svg width="28" height="24" viewBox="0 0 28 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M27.9172 2.16235L23.6922 22.0874C23.3732 23.4934 22.5422 23.8434 21.3612 23.1814L14.9232 18.4374L11.8172 21.4254C11.4732 21.7694 11.1862 22.0564 10.5232 22.0564L10.9862 15.5004L22.9172 4.71935C23.4362 4.25735 22.8042 4.00035 22.1112 4.46335L7.36124 13.7514L1.01124 11.7634C-0.369763 11.3324 -0.394763 10.3824 1.29924 9.71935L26.1362 0.150353C27.2862 -0.280647 28.2922 0.405353 27.9172 2.16235Z" fill="#0088CC"/>
                                </svg>
                            </div>
                            <div class="registration__alt-btns-btn">
                                <svg width="28" height="17" viewBox="0 0 28 17" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M26.672 16.508H23.6293C22.4787 16.508 22.132 15.576 20.0693 13.512C18.2667 11.7747 17.5053 11.5587 17.0493 11.5587C16.4187 11.5587 16.2467 11.732 16.2467 12.6V15.336C16.2467 16.076 16.0067 16.5093 14.0733 16.5093C12.1977 16.3833 10.3789 15.8135 8.76662 14.8469C7.15437 13.8802 5.79483 12.5444 4.8 10.9493C2.43785 8.00936 0.794277 4.55877 0 0.871997C0 0.415997 0.173333 0.00266357 1.04267 0.00266357H4.08267C4.864 0.00266357 5.14533 0.350664 5.452 1.15466C6.928 5.49866 9.44667 9.27733 10.4693 9.27733C10.8613 9.27733 11.032 9.104 11.032 8.12666V3.652C10.9027 1.61066 9.81867 1.43866 9.81867 0.699997C9.83238 0.505118 9.92152 0.323262 10.0672 0.193054C10.2128 0.0628473 10.4035 -0.00545217 10.5987 0.00266357H15.3773C16.0307 0.00266357 16.2467 0.327997 16.2467 1.10933V7.14933C16.2467 7.80133 16.5267 8.01733 16.724 8.01733C17.116 8.01733 17.4173 7.80133 18.136 7.084C19.6765 5.20531 20.935 3.11222 21.872 0.870664C21.9679 0.601535 22.1492 0.371163 22.3883 0.214686C22.6273 0.0582099 22.911 -0.0157821 23.196 0.0039968H26.2373C27.1493 0.0039968 27.3427 0.459997 27.1493 1.11066C26.0432 3.58855 24.6744 5.94067 23.0667 8.12666C22.7387 8.62666 22.608 8.88666 23.0667 9.47333C23.368 9.92933 24.4347 10.82 25.1507 11.6667C26.1933 12.7067 27.0587 13.9093 27.7133 15.2267C27.9747 16.0747 27.54 16.508 26.672 16.508Z" fill="#0077FF"/>
                                </svg>
                            </div>
                            <div class="registration__alt-btns-btn">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M8.2411 0.658116C10.9182 -0.242855 13.8292 -0.218074 16.49 0.728335C17.9511 1.26468 19.2899 2.07859 20.4295 3.12337C20.0423 3.5295 19.6338 3.90906 19.2389 4.3038C18.4878 5.03889 17.7373 5.77144 16.9875 6.50146C16.24 5.80056 15.3358 5.28065 14.3469 4.98322C13.0816 4.60867 11.7354 4.58302 10.4562 4.9091C9.17695 5.23517 8.01404 5.90036 7.09505 6.83168C6.29288 7.63168 5.68538 8.59895 5.3179 9.66131L1.30479 6.61533C2.74124 3.82283 5.22836 1.68677 8.2411 0.658116Z" fill="#E33629"/>
                                    <path d="M0.240046 9.63285C0.455587 8.58482 0.813701 7.56992 1.30479 6.61533L5.3179 9.6689C4.79306 11.1845 4.79306 12.8276 5.3179 14.3432C3.98084 15.3554 2.64314 16.3726 1.30479 17.3949C0.0757861 14.9966 -0.299038 12.2642 0.240046 9.63285Z" fill="#F8BD00"/>
                                    <path d="M12.2445 9.7562H23.767C24.1609 11.8759 24.0543 14.056 23.4553 16.129C22.904 18.0353 21.8332 19.7583 20.3579 21.1127C19.0628 20.122 17.7618 19.139 16.4667 18.1483C17.1088 17.7237 17.6568 17.1764 18.078 16.5392C18.4991 15.902 18.7847 15.188 18.9176 14.44H12.2445C12.2426 12.88 12.2445 11.3181 12.2445 9.7562Z" fill="#587DBD"/>
                                    <path d="M1.30285 17.3949C2.6412 16.3827 3.9789 15.3655 5.31596 14.3432C5.83325 15.8315 6.81707 17.1214 8.12688 18.0287C8.94373 18.595 9.87208 18.988 10.8526 19.1826C11.8187 19.3588 12.8097 19.3588 13.7758 19.1826C14.7392 19.023 15.6578 18.6674 16.4725 18.1388C17.7676 19.1295 19.0686 20.1125 20.3637 21.1032C18.9464 22.3666 17.2187 23.2475 15.3497 23.6595C13.2868 24.135 11.1371 24.1122 9.08515 23.5931C7.46229 23.1683 5.94644 22.4195 4.63259 21.3936C3.24209 20.3111 2.10632 18.9471 1.30285 17.3949Z" fill="#319F43"/>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div class="registration__login">
                        <span>Уже зарегистрированы? <a href="#">Войдите</a></span>
                    </div>

                </div>

                <div class="welcome">
                    <div class="welcome__title">
                        Добро пожаловать на платформу CHINASPACE!
                    </div>
                    <div class="welcome__desc">
                        Здесь вы можете заказать выкуп и доставку любых товаров из Китая. А также искать их на популярных китайских маркетплейсах через наш уникальный встроенный поиск по фото и по ключевым словам.
                    </div>
                    <video width="693" height="315" controls>
                        <source src="/nevergonna.mp4" type="video/mp4">
                    </video>
                </div>
            </div>
        </AppContainer>
    </main>
</template>




<style lang="scss" scoped>

input::-webkit-input-placeholder       {opacity: 1; transition: opacity 0.3s ease;}
input::-moz-placeholder                {opacity: 1; transition: opacity 0.3s ease;}
input:-moz-placeholder                 {opacity: 1; transition: opacity 0.3s ease;}
input:-ms-input-placeholder            {opacity: 1; transition: opacity 0.3s ease;}
input:focus::-webkit-input-placeholder {opacity: 0; transition: opacity 0.3s ease;}
input:focus::-moz-placeholder          {opacity: 0; transition: opacity 0.3s ease;}
input:focus:-moz-placeholder           {opacity: 0; transition: opacity 0.3s ease;}
input:focus:-ms-input-placeholder      {opacity: 0; transition: opacity 0.3s ease;}

.layer {
    display: flex;
    gap: 28px;
}

.registration {
    background: #F8F8F8;
    max-width: 388px;
    border-radius: 16px;
    padding-top: 32px;
    padding-right: 48px;
    padding-bottom: 32px;
    padding-left: 48px;
    border: 1px solid #F2F2F2;
    

    &__login {
        text-align: center;
        font-size: 14px;
        font-weight: 400;
        a {
            text-decoration: none;
            color: #66B359;
            font-weight: 700;
            transition: .2s ease;
            &:hover {
                transition: .2s ease;
                filter: brightness(120%);
            }

        }
    }

    &__alt {
        &-title {
            text-align: center;
            margin-bottom: 24px;
        }
        &-btns {
            display: flex;
            justify-content: space-between;
            padding-right: 50px;
            padding-left: 50px;
            margin-bottom: 32px;
            &-btn {
                width: 48px;
                height: 48px;
                border: 1px solid #D4D4D4;
                border-radius: 8px;
                display: flex;
                justify-content: center;
                align-items: center;
                transition: .2s ease;
                cursor: pointer;
                svg {
                    path {
                        transition: .2s ease;
                    }
                }
                &:hover {
                    border: 1px solid #404040;
                    background: #404040;
                    transition: .2s ease;
                    svg {
                        path {
                            fill: white;
                            transition: .2s ease;
                        }
                    }
                }
            }
        }
    }
    button {
        height: 52px;
        width: 100%;
        background: #404040;
        color: #FFFFFF;
        border-radius: 8px;
        outline: none;
        transition: .2s ease;
        cursor: pointer;
        margin-bottom: 24px;
        &:hover {
            color: #404040;
            border: 1px solid #404040;
            background: #F8F8F8;
            transition: .2s ease;
        }
    }

    &__title {
        font-size: 22px;
        font-weight: 600;
        margin-bottom: 32px;
    } 
    
    &__policy {
        font-size: 12px;
        font-weight: 400;
        color: #404040;
        display: flex;
        margin-bottom: 24px;
        input {
            margin-right: 8px;
            cursor: pointer;
            width: 16px;
            height: 16px;
        }
        a {
            text-decoration: none;
            color: #B4B4B4;
        }
        
    }

    &__form {
        div.input {
            margin-bottom: 16px;
        }
        input {
            width: 100%;
            height: 40px;
            border-radius: 8px;
            border: 1px solid #E6E6E6;
            padding: 12px;
            font-size: 12px;
            font-weight: 300;
            color: #7F8086;
            transition: .2s ease;
            outline: none;
            &:focus {
                border: 1px solid #404040;
                transition: .2s ease;
                
            }
        }
        &-title {
            font-size: 14px;
            font-weight: 400;
            margin-bottom: 8px;
        }
    }
}

.welcome {
    background: #F8F8F8;
    border: 1px solid #F2F2F2;
    border-radius: 16px;
    padding-top: 32px;
    padding-left: 48px;
    padding-right: 48px;
    padding-bottom: 37px;
    height: 100%;
    width: 100%;
    &__title {
        color: #2F2F2F;
        font-size: 22px;
        font-weight: 600;
        margin-bottom: 32px;
    }
    &__desc {
        color: #2F2F2F;
        font-size: 14px;
        font-weight: 400;
        margin-bottom: 32px;
    }
}

</style>