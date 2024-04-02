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
                    <li class="nav-link">
                        

                        <a href="#" class="navli">
                            <img src="/navnotifico.svg" alt="" class="navicons">
                            Уведомления</a>
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
}

.nav-link:hover a {
    background: #F2F2F2;
}
</style>