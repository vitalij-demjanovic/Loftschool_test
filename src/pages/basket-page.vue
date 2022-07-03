<template>
  <div class="basket-page">
    <div class="container">
      <h1 class="basket-title">КОРЗИНА</h1>
      <div class="basket-head">
        <span class="basket-head-span">Выделено</span>
        <div class="basket-head-delete">
          <button class="delete-btn">x</button>
          <span>удалить отмеченные</span>
        </div>
      </div>
      <div class="basket-result">
        <div class="basket-result-sum">
          <span>Промежуточный итог по корзине:</span>
          <div class="result-sum">0 p</div>
        </div>
        <div class="basket-result-nds">
          <span>В том числe НДС:</span>
          <div class="result-sum">0 p</div>
        </div>
      </div>
      <div class="basket-all-sum">
        <span>Итого:</span>
        0 p
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'baske-page'
}
</script>

<style lang="css">
.basket-title {
  color: #1f5d71;
  margin-bottom: 30px;
}

.basket-head {
  background: #d9e8ee;
  width: 100%;
  padding: 25px 20px;
  display: flex;
  justify-content: space-between;
}

.basket-head-span {
  font-size: 18px;
}

.basket-head-delete {
  cursor: pointer;
}

.basket-head-delete span {
  margin-left: 5px;
  border-bottom: 1px solid #000000;
}

.basket-head-delete:hover > .delete-btn {
  background: #ff0000;
}

.delete-btn {
  background: #9b8f8f;
  padding: 5px;
  border-radius: 5px;
  color: #ffff;
  transition: all 0.3s ease;
}

.basket-result {
  padding: 50px 0;
  margin-bottom: 20px;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  border-bottom: 1px dashed #000000;
  border-top: 1px solid #000000;
}
.basket-result-sum {
  margin-bottom: 20px;
}

.basket-result-sum,
.basket-result-nds {
  display: flex;
  width: 400px;
  justify-content: space-between;
}

.result-sum {
  font-weight: 700;
}

.basket-all-sum {
  color: #1f5d71;
  font-weight: 700;
  font-size: 20px;
  display: flex;
  justify-content: right;
}

.basket-all-sum span {
  font-weight: normal;
  margin-right: 10px;
}
</style>
