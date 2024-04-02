<template>
  <main>
    <AppContainer>
      <div class="content">
        <div class="leftsidegrid">
          <div class="gridblack">
            <blacksq title="Новый заказ" text="1688, TaoBao, Инвойс, добавление вручную" icon="plus"/>
            <blacksq title="Избранные товары" text="Список товаров, которые вы ранее сохранили" icon="packet"/>
            <blacksq title="Мои заказы" text="Подробная информация о размещенных заказах" icon="box"/>
            <blacksq title="С чего начать" text="Показываем как пользоваться платформой" icon="help"/>
          </div>
          <purchased class="purchasedsq" />
        </div>
        <div class="main">
          <div class="rightsidegrid">
            <mymanager />
            <greensq valueusers="456" title="пользователей" text="Приглашено по вашей реферально ссылке"/>
            <orangesq valuebonuses="15412" title="бонусов" text="Можно потратить на любой заказ"/>
          </div>
          <myorders />
        </div>
      </div>
    </AppContainer>
  </main>
</template>
<script>
import appContainer from '~/components/app-container.vue'

export default {
  components: { appContainer },

}
</script>

<style>


.rightsidegrid {
  display: flex;
  margin: -10px;
  margin-bottom: 10px;




}

.content {
  display: flex;
  gap: 20px;

}




.leftsidegrid {
  width: 388px;
  display: grid;
  gap: 20px;

}
.gridblack {
  display: grid;
  grid-template-columns: 184px 184px;
  grid-template-rows: 158px 158px;
  gap: 20px;
  width: 388px;
  top: 0px;
  left: 0px;
}








</style>
