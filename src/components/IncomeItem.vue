<template>
  <div class="income-item">
    <div class="removeItem"></div>
    <div class="desc">Description...</div>
    <div class="price">₽0</div>
    <div class="date">Date...</div>
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
.income-item {
    position: relative;
    display: flex;
    padding: 15px 15px 15px 0px;
    background-color: #FFF;
    border-radius: 8px;
    max-width: 600px;
    margin: 0 auto 30px;
}

.removeItem {
    color: #EF2D2D;
    font-weight: 600;
    font-size: 20px;
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
    max-width: 100px;
    font-size: 20px;
}

.date {
    color: #666;
    text-align: right;
    font-size: 20px;
}
</style>