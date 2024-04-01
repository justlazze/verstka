<template>
    <div class="navbar">
        <AppContainer>
                    <div class="brand-logo"> 
                <a href="/">
                    <img src="navbrandlogo.svg" alt="">
                </a>

            </div>
            <div class="nav-items">
                <ul class="nav-item">
                    <li class="nav-link">
                        <img src="/navneworderico.svg" alt="" class="navicons">

                        
                        <a href="#" class="navli">Новый заказ</a>
                    </li>
                    <li class="nav-link">
                        <img src="/navordersico.svg" alt="" class="navicons">

                        <a href="orders" class="navli">Заказы</a>
                    </li>
                    <li class="nav-link">
                        <img src="/navnotifico.svg" alt="" class="navicons">

                        <a href="#" class="navli">Уведомления</a>
                    </li>
                    <li class="nav-link">
                        <img src="/navhelpico.svg" alt="" class="navicons">
                        <a href="#" class="navli">Помощь</a>
                        
                    </li>
                    
                </ul>
                <HeaderProfile />
            </div>
            </AppContainer>
        </div>
    
    
</template>

<script>
import AppContainer from "~/components/app-container.vue"
export default {
    components: {
        AppContainer},
    props: {
        
    }

}
</script>

<style>

.navbar {
    display: flex;
    justify-content: center;
}

.navbar .app-container {
    margin: 0 auto;
    display: flex;
    height: 46px;
    margin-top: 20px;
    margin-bottom: 60px;
    align-items: center;
    justify-content: space-between;
}

.brand-logo {
    width: 166px;
    align-content: space-between;
    display: flex;
    align-items: center;
    vertical-align: middle;
    margin-top: 2px;
}

.brand-logo:hover {
    cursor: pointer;
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
    transition: .2s ease-in;
}

.nav-item {
    text-decoration: none;
}

a.navli {
    text-decoration: none;
    vertical-align: middle;
    color: #404040;
}

.navicons {
    max-height: 24px;
    max-width: 24px;
    margin: 0;
    vertical-align: middle;
    transition: .2s ease-in;
}

.nav-link a:after {
	display: flex;
	position: static;
	right: 0;
	width: 0;
	height: 1px;
	background-color: #404040;
	content: "";
	transition: width .2s ease-out; 
    margin-left: 29px;
}

.nav-link a:hover:after,
.nav-link a:focus:after {
	width: 10px;
}
</style>