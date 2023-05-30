
<script>
    export default {
        name: "Payments"
    } 
</script>

<template>
    <div class="payments-area">
        <div class="price">
            <h5>149.99</h5>
            <p>169.99</p>
        </div><!--price-->
        <button>
            <img src="../assets/icon-cart.svg" alt="cart icon">
            <span>Add to cart</span>
        </button>
    </div><!--payments-area-->
</template>

<style>
    .payments-area .price {
        display: flex;
        margin: 20px 0;
        display: flex;
        align-items: center;
    }
    .payments-area .price h5 {
        font-family: 'Fraunces', serif;
        font-size: 2em;
        color: #3c8067;
    }
    .payments-area .price p {
        margin-left: 15px;
        position: relative;
    }
    .payments-area .price p::before {
        content: '______';
        position: absolute;
        width: 100%;
        bottom: 5px;
    }

    .payments-area button {
        width: 235px;
        height: 48px;
        background-color: #3c8067;
        color: #ffff;
        border-radius: .7em;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        transition: .3s;
    }
    .payments-area button:hover {
        background-color: #1a4031;
    }

    @media (max-width: 650px) {
       .payments-area button {
        width: 305px;
       }
    }
</style>

