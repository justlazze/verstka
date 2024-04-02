<template>
<div class="navbar__profile" :class="{'opened': isShow}" @click="toggle">
    <div class="navbar__profile-photo">
        <img src="navbarphoto.svg" alt="">
    </div>
    <div class="navbar__profile-info">
        <div class="navbar__profile-info-name">
            Oleg K.
        </div>
        <div class="navbar__profile-info-id">
            ID: 000001
        </div>
    </div>
    <div class="navbar__profile-info-row">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M4 6L8 10L12 6" stroke="#404040" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
    </div>
    <div class="navbar__profile-menu">
        <div class="navbar__profile-menu-btns">
            <div class="navbar__profile-menu-btns-btn">
                    <svg class="stroke" width="22" height="20" viewBox="0 0 22 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M1.25 10.0002L10.205 1.04524C10.3094 0.940808 10.4333 0.857961 10.5697 0.801437C10.7061 0.744913 10.8523 0.71582 11 0.71582C11.1477 0.71582 11.2939 0.744913 11.4303 0.801437C11.5667 0.857961 11.6906 0.940808 11.795 1.04524L20.75 10.0002M3.5 7.75024V17.8752C3.5 18.4962 4.004 19.0002 4.625 19.0002H8.75V14.1252C8.75 13.5042 9.254 13.0002 9.875 13.0002H12.125C12.746 13.0002 13.25 13.5042 13.25 14.1252V19.0002H17.375C17.996 19.0002 18.5 18.4962 18.5 17.8752V7.75024M7.25 19.0002H15.5" stroke="#404040" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>

                <a href="#">Главный экран</a>
            </div>
            <div class="navbar__profile-menu-btns-btn">
                <svg class="fill" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M3.196 14.485C4.046 13.873 4.948 13.3893 5.902 13.034C6.85533 12.678 7.888 12.5 9 12.5C10.1113 12.5 11.144 12.678 12.098 13.034C13.0513 13.3893 13.9533 13.8727 14.804 14.484C15.464 13.8013 15.995 12.9947 16.397 12.064C16.799 11.132 17 10.1107 17 9C17 6.78333 16.221 4.89567 14.663 3.337C13.105 1.77833 11.2173 0.999333 9 1C6.78333 1 4.89567 1.77933 3.337 3.338C1.77833 4.89667 0.999333 6.784 1 9C1 10.1113 1.201 11.1323 1.603 12.063C2.005 12.9943 2.536 13.8017 3.196 14.485ZM9.001 9.5C8.15833 9.5 7.44733 9.21067 6.868 8.632C6.28933 8.054 6 7.34367 6 6.501C6 5.65833 6.28933 4.94733 6.868 4.368C7.446 3.78933 8.15633 3.5 8.999 3.5C9.84167 3.5 10.5527 3.78933 11.132 4.368C11.7107 4.946 12 5.65633 12 6.499C12 7.34167 11.7107 8.05267 11.132 8.632C10.554 9.21067 9.84367 9.5 9.001 9.5ZM9 18C7.74467 18 6.56967 17.7663 5.475 17.299C4.38033 16.8323 3.42767 16.1937 2.617 15.383C1.807 14.5723 1.16833 13.6197 0.701 12.525C0.233667 11.4303 0 10.2553 0 9C0 7.74467 0.233667 6.56967 0.701 5.475C1.16767 4.38033 1.80633 3.42767 2.617 2.617C3.42767 1.807 4.38033 1.16833 5.475 0.701C6.56967 0.233667 7.74467 0 9 0C10.2553 0 11.4303 0.233667 12.525 0.701C13.6197 1.16767 14.5723 1.80633 15.383 2.617C16.193 3.42767 16.8317 4.38033 17.299 5.475C17.7663 6.56967 18 7.74467 18 9C18 10.2553 17.7663 11.4303 17.299 12.525C16.8323 13.6197 16.1937 14.5723 15.383 15.383C14.5723 16.193 13.6197 16.8317 12.525 17.299C11.4303 17.7663 10.2553 18 9 18ZM9 17C9.922 17 10.829 16.8387 11.721 16.516C12.6137 16.194 13.385 15.7527 14.035 15.192C13.385 14.6707 12.633 14.2583 11.779 13.955C10.9257 13.6517 9.99933 13.5 9 13.5C8.00133 13.5 7.072 13.6483 6.212 13.945C5.352 14.2417 4.603 14.6573 3.965 15.192C4.615 15.752 5.38633 16.1933 6.279 16.516C7.171 16.8387 8.078 17 9 17ZM9 8.5C9.56133 8.5 10.035 8.307 10.421 7.921C10.807 7.535 11 7.06133 11 6.5C11 5.93867 10.807 5.465 10.421 5.079C10.035 4.693 9.56133 4.5 9 4.5C8.43867 4.5 7.965 4.693 7.579 5.079C7.193 5.465 7 5.93867 7 6.5C7 7.06133 7.193 7.535 7.579 7.921C7.965 8.307 8.43867 8.5 9 8.5Z" fill="#404040"/>
                </svg>
                <a href="#">Мой профиль</a>
            </div>
            <div class="navbar__profile-menu-btns-btn">
                <svg class="stroke" width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16 8.91553L6 3.35717M12.4171 1.36588L19.56 5.33594C19.9975 5.57904 20.3611 5.93035 20.614 6.35425C20.8669 6.77815 21.0001 7.25956 21 7.74967V14.2502C21.0001 14.7403 20.8669 15.2217 20.614 15.6456C20.3611 16.0695 19.9975 16.4208 19.56 16.6639L12.4171 20.634C11.9855 20.8738 11.4971 20.9999 11 20.9999C10.5029 20.9999 10.0145 20.8738 9.58286 20.634L2.44 16.6639C2.00249 16.4208 1.63885 16.0695 1.38596 15.6456C1.13306 15.2217 0.999911 14.7403 1 14.2502V7.74967C0.999911 7.25956 1.13306 6.77815 1.38596 6.35425C1.63885 5.93035 2.00249 5.57904 2.44 5.33594L9.58286 1.36588C10.0145 1.12606 10.5029 0.999924 11 0.999924C11.4971 0.999924 11.9855 1.12606 12.4171 1.36588Z" stroke="#404040" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.5 6.49992L9.68739 11.1859C10.0908 11.4055 10.5418 11.5205 11 11.5205C11.4582 11.5205 11.9092 11.4055 12.3126 11.1859L20.5 6.49992M11 11.8999V20.9999" stroke="#404040" stroke-linecap="round" stroke-linejoin="round"/>
</svg>


                <a href="#">Мои заказы</a>
            </div>
            <div class="navbar__profile-menu-btns-btn">
                <svg class="fill" width="18" height="20" viewBox="0 0 18 20" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M13.4216 4.16399C13.4184 4.10908 13.4142 4.05443 13.4089 4.00007C13.1934 1.75529 11.3021 0 9.00084 0C6.69956 0 4.80825 1.75529 4.59273 4.00007C4.58751 4.05443 4.58327 4.10908 4.58004 4.16399H1H0V5.16399V14C0 17.3137 2.68629 20 6 20H12C15.3137 20 18 17.3137 18 14V5.16399V4.16399H17H13.4216ZM9.00084 1C7.2524 1 5.80965 2.30876 5.59878 4.00007H12.4029C12.192 2.30876 10.7493 1 9.00084 1ZM1 5.16399H17V14C17 16.7614 14.7614 19 12 19H6C3.23858 19 1 16.7614 1 14V5.16399Z" fill="#404040"/>
</svg>

                <a href="#">Избранные товары</a>
            </div>
            <div class="navbar__profile-menu-btns-btn">
                <svg class="fill" width="22" height="14" viewBox="0 0 22 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M21.9434 6.63585C21.8988 6.7812 21.8278 6.91561 21.7343 7.03128C21.6409 7.14695 21.527 7.24157 21.3992 7.30965L19.1986 8.49L14.1608 13.8901C14.116 13.9367 14.0607 13.9702 14.0003 13.9872C13.94 14.0042 13.8765 14.0043 13.8161 13.9873L8.01087 12.4317C7.9664 12.4201 7.92448 12.3993 7.88751 12.3704L2.82971 8.50167L0.601957 7.30673C0.474076 7.23824 0.360035 7.14342 0.266345 7.02768C0.172656 6.91194 0.101153 6.77755 0.0559214 6.63219C0.0106894 6.48682 -0.00738602 6.33333 0.00272723 6.18048C0.0128405 6.02763 0.0509443 5.87841 0.114863 5.74135L2.36801 0.911026C2.43191 0.773951 2.52037 0.651709 2.62835 0.551283C2.73632 0.450857 2.8617 0.374213 2.99731 0.325729C3.13292 0.277245 3.27611 0.25787 3.41871 0.26871C3.56131 0.279551 3.70052 0.320394 3.82839 0.388909L5.95637 1.5294L10.8999 0.0145782C10.9652 -0.00485939 11.0341 -0.00485939 11.0994 0.0145782L16.0429 1.5294L18.1709 0.388909C18.2988 0.320394 18.438 0.279551 18.5806 0.26871C18.7232 0.25787 18.8664 0.277245 19.002 0.325729C19.1376 0.374213 19.263 0.450857 19.371 0.551283C19.4789 0.651709 19.5674 0.773951 19.6313 0.911026L21.8844 5.74232C21.9488 5.87918 21.9872 6.0284 21.9973 6.18129C22.0074 6.33418 21.9891 6.4877 21.9434 6.63294V6.63585ZM0.92578 6.61155L2.85511 7.64509L5.43299 2.11861L3.50457 1.08507C3.46198 1.06214 3.4156 1.04844 3.36808 1.04473C3.32055 1.04102 3.27281 1.04738 3.22758 1.06345C3.18235 1.07952 3.14051 1.10499 3.10446 1.13839C3.06841 1.1718 3.03885 1.21248 3.01747 1.25813L0.764322 6.08943C0.742936 6.13507 0.730148 6.18479 0.726689 6.23573C0.723229 6.28667 0.729165 6.33785 0.744158 6.38633C0.759151 6.43482 0.782908 6.47966 0.814071 6.5183C0.845233 6.55695 0.883192 6.58863 0.92578 6.61155ZM16.9863 9.75495L13.9222 7.12394C12.2414 8.75349 10.0418 9.02087 8.23854 7.78607C8.10075 7.69243 7.98436 7.56678 7.89798 7.41843C7.81159 7.27007 7.75743 7.10279 7.73949 6.92897C7.72155 6.75515 7.74029 6.57923 7.79433 6.41422C7.84837 6.24921 7.93632 6.09933 8.05169 5.97567L12.197 1.66552C12.265 1.59474 12.3562 1.5553 12.451 1.55565H13.4886L10.9997 0.79338L6.17315 2.27126L3.48098 8.04372L8.25215 11.6966L13.7907 13.1813L16.9863 9.75495ZM18.5392 8.09039L15.8552 2.33348H12.5979L8.56237 6.52987C8.52479 6.57024 8.49621 6.6192 8.47877 6.67308C8.46134 6.72696 8.45549 6.78436 8.46168 6.84101C8.46747 6.9 8.48555 6.95684 8.5146 7.00733C8.54365 7.05782 8.58291 7.10066 8.62949 7.13269C9.89485 7.999 11.8768 8.24499 13.6447 6.33542C13.7078 6.26733 13.7922 6.22668 13.8816 6.2213C13.971 6.21591 14.0592 6.24617 14.129 6.30625L17.5042 9.20366L18.5392 8.09039ZM21.2341 6.08943L18.9818 1.25813C18.9605 1.21248 18.9309 1.1718 18.8948 1.13839C18.8588 1.10499 18.817 1.07952 18.7717 1.06345C18.7265 1.04738 18.6787 1.04102 18.6312 1.04473C18.5837 1.04844 18.5373 1.06214 18.4947 1.08507L16.5663 2.11861L19.1442 7.64509L21.0735 6.61155C21.1161 6.58863 21.1541 6.55695 21.1852 6.5183C21.2164 6.47966 21.2402 6.43482 21.2551 6.38633C21.2701 6.33785 21.2761 6.28667 21.2726 6.23573C21.2692 6.18479 21.2555 6.13507 21.2341 6.08943Z" fill="#404040"/>
                </svg>
                <a href="#">Партнерам</a>
            </div>
            <div class="navbar__profile-menu-btns-btn">
                <svg class="stroke" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M16.005 2.02217L2.01826 16.1643M7.66667 4.33333C7.66667 6.17428 6.17428 7.66667 4.33333 7.66667C2.49238 7.66667 1 6.17428 1 4.33333C1 2.49238 2.49238 1 4.33333 1C6.17428 1 7.66667 2.49238 7.66667 4.33333ZM17 13.6667C17 15.5076 15.5076 17 13.6667 17C11.8257 17 10.3333 15.5076 10.3333 13.6667C10.3333 11.8257 11.8257 10.3333 13.6667 10.3333C15.5076 10.3333 17 11.8257 17 13.6667Z" stroke="#404040" stroke-linecap="round"/>
                </svg>
                <a href="#">Акции</a>
            </div>
        </div>
        <div class="navbar__profile-menu-selectacc">
            <div class="navbar__profile-menu-selectacc-another">
                <a href="#">Войти в другой аккаунт</a>
            </div>
            <div class="navbar__profile-menu-selectacc-account">
                <div class="navbar__profile-menu-selectacc-account-photo">
                    <img src="navbarphoto.svg" alt="">
                </div>
                <div class="navbar__profile-menu-selectacc-account-info">
                    <div class="navbar__profile-menu-selectacc-account-info-name">
                        Oleg K.
                    </div>
                    <div class="navbar__profile-menu-selectacc-account-info-id">
                        ID: 000001
                    </div>
                </div>
    </div>



        </div>
        <div class="navbar__profile-menu-exit">
            <div class="navbar__profile-menu-btns-btn">
                <svg class="stroke" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M6.33333 17H2.77778C2.30628 17 1.8541 16.8127 1.5207 16.4793C1.1873 16.1459 1 15.6937 1 15.2222V2.77778C1 2.30628 1.1873 1.8541 1.5207 1.5207C1.8541 1.1873 2.30628 1 2.77778 1H6.33333M12.5556 13.4444L17 9M17 9L12.5556 4.55556M17 9H6.33333" stroke="#404040" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>

                <a href="#">Выход</a>
            </div>
        </div>
    </div>
</div>
</template>

<script>

export default {
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
        }
    }
}
</script>

<style lang="scss" scoped>
.navbar__profile {
    width: 213px;
    height: 46px;
    background: #F8F8F8;
    border-radius: 8px;
    display: flex;
    align-items: center;
    padding: 8px;
    cursor: pointer;
    position: relative;
    z-index: 10;
    transition: .2s ease-out;
    $root: &;
    &:hover {
        background: #eeeeee;
        transition: .2s;
        #{$root} {
            &info-row {
                transition: .2s;
            }
        }
    }
    &.opened {
        height: auto;
        border-radius: 8px 8px 0 0;
        filter: drop-shadow(0px 1px 5.7px rgba(69, 69, 69, 0.2));
        .navbar__profile-info-row {
            transform: scale(-1);
            transition: .2s ease-out;
        }
        &:hover {
            background: #F8F8F8;
        }
        #{$root} {
            &-menu {
                display: block;
            }
        }
    }

    &-menu-btns-btn svg {
        max-height: 24px;
        max-width: 24px;
        margin: 8px;
        flex: 1;

    }

    &-menu-btns {
        border-bottom: #D4D4D4 solid 1px;
        align-items: center;
        padding-bottom: 6px;
        margin: 4px;
       
    }

    &-menu-btns-btn {
        height: 40px;
        background: #FFFFFF;
        display: flex;
        margin: 8px;
        margin-left: 4px;
        margin-right: 4px;
        align-items: center;
        border-radius: 4px;
        font-size: 14px;
        font-weight: 600;
        transition: .2s ease-out;
        
        &:hover {
            background: #404040;
            transition: .2s ease-out;
            cursor: pointer;
        }
        &:hover a{
            color: white;
            transition: .2s ease-out;
        }
        &:hover svg.fill path {
            fill: white;
            transition: .2s ease-out;
        }
        &:hover svg.stroke path {
            stroke: white;
            transition: .2s ease-out;
        }
        
        
        
    }

   

    &-menu a {
        text-decoration: none;
        color: #404040;
    }

    &-info {
        &-row {
        transition: .2s ease-out;
        }
    }

        
    
    &-info {
        margin-left: 12px;
        flex: auto;
    }
    &-info-id {
        font-size: 12px;
        font-weight: 400;
        color: #7F8086;
    }
    &-info-name {
        font-size: 14px;
        color: #404040;
        font-weight: 600;
    }
    &-info-photo {
        img {
            display: block;
        }
    }
    &-menu {
        position: absolute;
        top: 100%;
        right: 0;
        background: #F8F8F8;
        border-radius: 0 0 8px 8px;
        z-index: 10;
        display: none;
        width: 100%;
        cursor: default;
        
        &-exit .navbar__profile-menu-btns-btn {
            margin-bottom: 4px;
        }


        &-selectacc {
            margin: 4px;
            margin-top: 12px;
        

        &-another {
            text-align: center;
            color: #7F8086;
            font-size: 12px;
            font-weight: 400;

            &:hover a {
                color: black;
            }
        }
        &-account {
            background: #F8F8F8;
            border-radius: 8px;
            display: flex;
            align-items: center;
            padding: 4px;
            opacity: 50%;
            margin-top: 4px;

            &-info {
                margin-left: 12px;
                flex: auto;
    
            &-id {
                font-size: 12px;
                font-weight: 400;
                color: #7F8086;
    }
            &-name {
                font-size: 14px;
                color: #404040;
                font-weight: 600;
    }
            &-photo {
                img {
                display: block;
        }
    }
}
        }
           
        }
    }
}
</style>