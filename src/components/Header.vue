<template>
    <header>
        <h1>Income Tracker</h1>
        <div class="total-income">£{{ totalIncome }} </div>
    </header>
</template>

<script>
export default {
    props: {
        totalIncome: Number
    }
}
</script>

<style scoped>
header {
    padding: 15px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #313131;
    border-bottom: 5px solid #FFCE00
}

h1 {
    color: #EEE;
    font-size: 28px;
}

.total-income {
    padding: 5px 10px;
    min-width: 100px;
    color: #FFF;
    background-color: #FFCE00;
    text-align: center;
    font-size: 20px;
    font-weight: 900;
    border-radius: 8px;
    box-shadow: inset 0px 0px 6px rgba(0, 0, 0, 0.25);
    text-shadow: 0px 3px 3px rgba(0, 0, 0, 0.25);
}
</style>