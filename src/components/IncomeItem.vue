<template>
  <div class="income-item">
    <div class="removeItem">x</div>
    <div class="desc">{{ income.desc }}</div>
    <div class="price">₽{{ income.value }}</div>
    <div class="date">{{ income.date }}</div>
  </div>
</template>

<script>
export default {
    props: {
        income: Object
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@500&family=Poppins:wght@300&display=swap');
.income-item {
    position: relative;
    display: flex;
    padding: 15px 15px 15px 0px;
    background-color: #FFF;
    border-radius: 8px;
    max-width: 600px;
    font-family: 'Poppins', sans-serif;
    margin: 0 auto 30px;
}

.removeItem {
    color: #EF2D2D;
    font-weight: 900;
    font-size: 25px;
    line-height: 1;
    text-align: center;
    margin: 0 15px;
}

.desc {
    color: #666;
    flex: 1 1 100%;
    font-size: 20px;
}

.price {
    color: #666;
    min-width: 100px;
    font-size: 20px;
}

.date {
    color: #666;
    text-align: right;
    font-size: 20px;
}
</style>