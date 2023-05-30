
<script>
    import Payments from './Payments.vue'

    export default {
        name: "MainInformation",
        components: {
            Payments
        }
    }
</script>

<template>
    <section>
        <p>PERFUME</p>
        <h1>Gabrielle Essence Eau De Parfum</h1>
        <p>A floral, solar and voluptuous interpretation composed by Oliver Polge, Perfumer-Creator for the House of CHANEL. </p>
        <payments/>
    </section>
</template>

<style>
    section {
        width: 300px;
        height: 450px;
        padding: 30px;
    }
    section h1 {
        font-family: 'Fraunces', serif;
        margin: 15px 0;
        font-size: 2em;
    }
    section p {
        line-height: 24px;
        color: #6c7289;
    }

    @media (max-width: 650px) {
        section {
            padding: 20px;
        }
        section h1 {
            font-size: 1.5em;
        }
        section p {
            font-size: 1em;
        }
    }

</style>