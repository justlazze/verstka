<template>
    <div class="mymanager">
        <div class="mymanager__textandbtn">
            <div class="mymanager__text">
            Мой менеджер
            </div>
            <div class="mymanager__buttons">
                <div class="mymanager__buttons-btn">
                W/A
                </div>
                <div class="mymanager__buttons-btn">
                TG
                </div>

            </div>
        </div>
        <div class="mymanager__photoinfo">
        <div class="mymanager__photo">
            <img src="mymanagerphoto.svg" alt="">
        </div>
        <div class="mymanager__info">
            <div class="mymanager__info-name aboutmanager">
                Юрий Михайлов
            </div>
            <div class="mymanager__info-number aboutmanager">
                8(800)333-52-62

            </div>
            <div class="mymanager__info-email aboutmanager">
                abababa@gmail.com

            </div>
        </div>
    </div>

    </div>
     
</template>



<style>
.mymanager__buttons-btn:hover {
    background: #404040;
    
    color: white;
    transition: .2s;

}

.mymanager__buttons-btn {
    cursor: pointer;
    transition: .2s;

}
.mymanager__info-email{
    font-size: 12px;
    font-weight: 400;
    color: #7F8086;
    cursor: pointer;
}

.mymanager__info-number {
    font-size: 12px;
    font-weight: 400;
    color: #7F8086;
    margin-bottom: 4px;
    cursor: pointer;
}

.mymanager__info-name {
    font-size: 14px;
    font-weight: 600;
    color: #404040;
    margin-bottom: 8px;
    cursor: pointer;
}

.aboutmanager:after {
	display: block;
	left: 0;
	width: 0;
	height: 1px;
    border-radius: 1px;
	background-color: #404040;
	content: "";
	transition: width .2s ease-out; 
}

.aboutmanager:hover:after,
.aboutmanager:focus:after {
	width: 10px;
}


.mymanager__photo {
    margin-right: 12px;
}

.mymanager__textandbtn {
    justify-content: space-between;
    display: flex;

}

.mymanager__photoinfo {
    display: flex;
    align-items: center;

}

.mymanager__buttons {
    width: 80px;
    display: flex;
    justify-content: space-between;

}

.mymanager__buttons-btn {
    border: 1px solid #404040;
    width: 36px;
    height: 36px;
    border-radius: 8px;
    font-size: 11px;
    font-weight: 600;
    justify-content: center;
    align-items: center;
    display: flex;

}


.mymanager {
    width: 384px;
    height: 158px;
    background: #F8F8F8 url(/mymanagerbg.svg) center center no-repeat;
    border-radius: 16px;
    margin: 10px;
    padding: 16px;
    justify-content: space-between;
}
</style>