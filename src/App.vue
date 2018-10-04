<template lang="pug">
div
    header.header
        span.logo
            | LOGO
        a.button1(href='something') Login
        a.button1(href='something') Create Account
    section.grid-wrapper
        .grid
            - var i = 0;
            while i < 6
                - i++
                .grid-cell
                    .grid-cell-inner
    footer.footer Bottom Nav

</template>

<script>

  export default {
    name: 'app',
    components: {}
  }
</script>

<style lang="scss">
    @import "grid.css";

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        background: #cba550;
    }
    .logo {
        float: left;
        padding: .5em;
    }

    .header {
        text-align: right;
        padding: .6em;
        background: #B2B2B2;
    }

    .footer {
        padding: 20px;
        background: #B2B2B2;
        text-align: center;
    }

    a.button1 {
        display: inline-block;
        padding: 0.35em 1.2em;
        border: 0.1em solid #FFFFFF;
        margin: 0 0.5em 0.1em 0;
        border-radius: 0.12em;
        box-sizing: border-box;
        text-decoration: none;
        font-family: 'Roboto', sans-serif;
        font-weight: 300;
        color: #FFFFFF;
        text-align: center;
        transition: all 0.2s;
    }

    a.button1:hover {
        color: #000000;
        background-color: #FFFFFF;
    }

    @media all and (max-width: 30em) {
         a.button1 {
            display: block;
            margin: 0.4em auto;
        }
    }
</style>
