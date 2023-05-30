<script>
    import MainInformations from "../components/mainInformations.vue"
    
    export default {
        name: "MainComponent",
        components: {
            MainInformations
        }
    }
</script>


<template>
    <main>
        <div class="main-container">
            <div class="perfum-img">
                
            </div><!--perfum-img-->
            <main-informations/><!--main-container-->
        </div>
    </main>
</template>


<style>
    main {
        width: 600px;
        height: 450px;
        background-color:  #fff;
        border-radius: .7em;
    }
    main .main-container {
        display: flex;
    }
    main .main-container .perfum-img {
        background-image: url("../assets/image-product-desktop.jpg");
        background-size: cover;
        height: 450px;
        width: 300px;
        border-radius: .7em 0 0 .7em;
    }
    @media (max-width: 650px) {
        main {
            height: 610px;
            width: 345px;
        }
        main .main-container .perfum-img {
            background-image: url("../assets/image-product-mobile.jpg");
        }
        main .main-container {
            flex-direction: column
        }
        main .main-container .perfum-img {
        background-image: url("../assets/image-product-desktop.jpg");
        background-size: 100%;
        background-position-y: 45%;
        height: 240px;
        width: 345px;
        border-radius: .7em 0 0 .7em;
        border-radius: 1em 1em 0 0;
        }
    }
</style>