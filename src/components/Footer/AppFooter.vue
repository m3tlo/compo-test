<template>
  <footer class="footer">
    <div class="container">
      <section class='footer__contacts'>

        <div class='footer__contacts-block'>
          <AppLogo width='205' height='40' class='footer__logo'/>

          <div class='contact'>
            <h5>8 800 841-95-95</h5>
            <p class="subtitle">Служба поддержки</p>
          </div>
          <div  class='contact'>
            <h5><a href='mailto:support@sport.ru'>support@sport.ru</a></h5>
            <p class="subtitle">Служба поддержки</p>
          </div>
        </div>
        <div>
          <menu class="footer__menu">
            <li class="footer__menu-item"><h5><a href="#" >Вакансии</a></h5></li>
            <li class="footer__menu-item"><h5><a href="#" >Блог</a></h5></li>
            <li class="footer__menu-item"><h5><a href="#" >Акции</a></h5></li>
            <AppButton class='light-blue'>Предложить идею</AppButton>
          </menu>
        </div>
      </section>
      <section class='footer__nav'></section>
      <section></section>
    </div>
  </footer>
</template>

<script setup>
import AppLogo from '@/components/icons/AppLogo.vue'
import AppButton from '@/components/UI/AppButton.vue'
</script>

<style scoped>
@import url("./footer.css");
.contact{
  display: flex;
  flex-direction: column;
  gap: 16px ;
}


</style>
