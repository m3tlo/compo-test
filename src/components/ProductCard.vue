<template>
  <div class="product">
    <AppBreadcrumbs />
    <h2 class="product__title pro">Кроссовки мужские Skechers Sunny Dale</h2>
    <div class="product__card">
      <div class="product__photo-carousel">
        <img
          width="400"
          height="400"
          src="@/assets/icons/Rectangle 1.png"
          alt=""
          class="product__photo-main"
        />
        <div class="product__photo-slider slider">
          <AppButton class="light-blue"><i class="fi fi-rr-angle-left"></i></AppButton>

          <ul class="slider__photo">
            <li class="slider__item">
              <img src="@/assets/icons/sneakers.png" alt="" class="slider__img" />
            </li>
            <li class="slider__item">
              <img src="@/assets/icons/sneakers.png" alt="" class="slider__img" />
            </li>
            <li class="slider__item">
              <img src="@/assets/icons/sneakers.png" alt="" class="slider__img" />
            </li>
            <li class="slider__item">
              <img src="@/assets/icons/sneakers.png" alt="" class="slider__img" />
            </li>
          </ul>
          <AppButton class="light-blue"><i class="fi fi-rr-angle-right"></i></AppButton>
        </div>
      </div>
      <div class="product__data">
        <div class="product__property">
          <div class="product__price">
            <div class='product__price-info'>
              <p class='red'>
                166 534.00 цена без скидки
              </p>
              <div class='row'>
              <h1 class='price'>122 566 ₽ </h1>
              <h5  class='sales__marker'>-15%</h5>
              </div>
              <div class='row'>
              <p class='amount-in-pack'>12 штук в уп.</p>
              <AppCheckbox>Заказ упаковкой</AppCheckbox>
              </div>
            </div>
            <div class='product__price-buy'>
              <div class='product__amount'>
                <div>
                  <h6>Завтра</h6>
                  <p class="subtitle">Доставка</p>
                </div>
                <div>
                  <h6>7 шт.</h6>
                  <p class="subtitle">Тарасовка</p>
                </div>
                <div>
                  <h6>7 шт.</h6>
                  <p class="subtitle">Тарасовка</p>
                </div>
              </div>
              <div class='product__buy'>
                <AppButton class='blue'>
                  <i class="fi fi-br-shopping-cart"></i>
                  В корзину
                </AppButton>

                <AppButton class='light-blue'>
                  <i class="fi fi-rr-heart"></i>
                </AppButton>
              </div>
            </div>
          </div>
          <div class="product__characteristic">
            <h4 class="product__characteristic-title">Характеристики</h4>
            <div class="row">
              <div class="col">
                <div>
                  <h6>ELC00696</h6>
                  <p class="subtitle">Код поставщика</p>
                </div>
                <div>
                  <h6>ELC00696</h6>
                  <p class="subtitle">Код РАЭК</p>
                </div>
                <div>
                  <h6>Electric used</h6>
                  <p class="subtitle">Бренд</p>
                </div>
                <div>
                  <h6>ELC0200000696</h6>
                  <p class="subtitle">Код производителя</p>
                </div>
              </div>
              <div class="col">
                <div>
                  <h6>ELC0200000696</h6>
                  <p class="subtitle">Артикул</p>
                </div>
                <div>
                  <h6>ELC00696</h6>
                  <p class="subtitle">Код ЕТМ</p>
                </div>
                <div>
                  <h6>ELC00696</h6>
                  <p class="subtitle">Серия</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="product__description">
          <h3 class="product__description-title">Описание товара</h3>
          <p class="product__description-text">
            Создание приверженного покупателя специфицирует неопровержимый комплексный анализ
            ситуации. CTR существенно индуцирует из ряда вон выходящий SWOT-анализ. Воздействие на
            потребителя определяет возрастающий интеграл по поверхности, что известно даже
            школьникам. Отсюда естественно следует, что коммуникация уравновешивает косвенный фактор
            коммуникации. Поле направлений естественно допускает экспериментальный скачок функции,
            таким образом сбылась мечта идиота - утверждение полностью доказано. Арифметическая
            прогрессия притягивает линейно зависимый пул лояльных изданий.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import AppBreadcrumbs from '@/components/UI/AppBreadcrumbs.vue'
import AppButton from './UI/AppButton.vue'
import AppCheckbox from './UI/AppCheckbox.vue'
</script>

<style scoped>


.product {
  max-width:1600px;
  margin: 0 auto;
  .product__title {
    text-transform: uppercase;
    margin-bottom: 32px;
  }
  img {
    border-radius: 16px;
  }
  .product__card {
    display: flex;
    .product__data {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      gap: 48px;
      .product__property {
        justify-content: space-between;
        max-width: 1100px;
        display: flex;
        gap:32px;
        .product__price {
          width: 372px ;
          height: 312px;
          display: flex;
          flex-direction: column;

          .product__price-buy, .product__price-info{
            display: flex;
            flex-direction: column;
            gap: 32px;
          }
          .product__price-info{
            margin-bottom: 32px;

            .row{
              gap: 12px;
              align-items: center;
              box-sizing: border-box;
            }
          }
          .product__amount, .product__buy{
            align-items: center;
            display: flex;
          }
          .product__amount{
            padding-top: 32px;
            box-sizing: border-box;
            border-top: 1px solid #e2e4f0 ;
            gap:16px;
            div{
              width: 115px;
              display: flex;
              flex-direction: column;
              gap: 4px;
            }
          }
          .product__buy{

            gap: 16px;
            .light-blue, .blue{
              flex: 1 1 auto;
              height: 56px;
              min-width: 72px;
            }
            .light-blue{
              width: 72px;
              flex-grow: 0;
            }
          }
        }
        .product__characteristic{
          padding-left: 48px ;
          border-left:1px solid #e2e4f0;

          .row{
            width: 800px;
            justify-content: space-between;
            height: 294px;
            gap: 32px;

          }
          .col{
            width: 302px;
            gap: 32px;

          h6{
            margin-bottom: 8px;
          }
          }
          .product__characteristic-title{
            margin-bottom: 32px;
          }
      }
      }
      .product__description {
        p {
          font-size: 18px;
        }
      }
    }
  }

  .product__photo-main {
    margin: 0px 48px 24px 0;
  }

  .slider {
    display: flex;
    align-items: center;
    gap: 12px;
    height: 64px;

    .slider__photo {
      display: flex;
      gap: 12px;

      .slider__item {
        list-style: none;
        img {
          width: 64px;
          height: 64px;
        }
      }
    }
  }
}
.light-blue {
  height: 100%;
}
.subtitle {
  font-size: 12px;
  line-height: 16px;
  color: #828ead;
  font-weight: 400;
}

.fi-br-shopping-cart:before {
  color: #fff;
  content: "\f9dc";
}
.fi-rr-heart:before{
  color: #1551E5;
  font-size: 18px;
}

</style>
