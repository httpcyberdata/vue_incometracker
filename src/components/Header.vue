<template>
  <header>
    <h1>Income Tracker</h1>
    <div class="total-income">₽0</div>
  </header>
</template>

<script>
export default {

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@500&family=Poppins:wght@300&display=swap');
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 35px 30px;
        background-color: #313131;
        border-bottom: 5px solid #FFCE00;
    }

    header h1 {
        color: #EEE;
        font-size: 40px;
        font-family: 'Fira Code', sans-serif;
    }
    header .total-income {
        font-family: 'Fira Code', sans-serif;
        background-color: #FFCE00;
        color: #FFF;
        font-size: 40px;
        font-weight: 900;
        padding: 3px 60px;
        min-width: 100px;
        text-align: center;
        border-radius: 8px;
        box-shadow: inset 0px 0px 6px rgba(0, 0, 0, 0.25);
        text-shadow: 0px 3px 3px rgba(0, 0, 0, 0.25);
    }
</style>