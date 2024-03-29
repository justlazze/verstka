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
                <div class="navbar__profile">
                    <div class="navbar__profile-photo">
                        <img src="navbarphoto.svg" alt="">
                    </div>
                    <div class="navbar__profile-info">
                        <div class="navbar__profile-name">
                            Oleg K.
                        </div>
                        <div class="navbar__profile-id">
                            ID: 000001
                        </div>

                    </div>
                    <div class="navbar__profile-row">
                        <img src="/navbarprofilerow.svg" alt="">

                    </div>

                </div>
                
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
.navbar__profile-row {
    transition: .2s ease-out;
}

.navbar__profile:hover .navbar__profile-row {
    transition: .2s;
    transform: scale(1.1);

}


.navbar__profile-info {
    margin-left: 12px;
    flex: auto;
}

.navbar__profile-id {
    font-size: 12px;
    font-weight: 400;
    color: #7F8086;
}

.navbar__profile-name {
    font-size: 14px;
    color: #404040;
    font-weight: 600;
}

.navbar__profile-photo img {
    display: block;
}

.navbar {
    display: flex;
    justify-content: center;
}

.navbar__profile {
    width: 213px;
    height: 46px;
    background: #F8F8F8;
    border-radius: 8px;
    display: flex;
    align-items: center;
    padding: 8px;
    cursor: pointer;
    transition: .2s;


}
.navbar__profile:hover {
background: #eeeeee;
transition: .2s;
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
    
}



.nav-item {
    text-decoration: none;

}


a.navli {
    text-decoration: none;
    vertical-align: middle;
}

.navicons {
    max-height: 24px;
    max-width: 24px;
    margin: 0;
    vertical-align: middle;
}
</style>