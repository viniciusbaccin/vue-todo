<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/icon-256-light.png" alt="">
                <h1> Vue Todo </h1>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">Inicio</RouterLink>
                <RouterLink to="/about">Sobre</RouterLink>
            </ul>
        </nav>
    </header>
</template>

<script setup>
import { RouterLink } from 'vue-router';

</script>

<style lang="scss" scoped>
header {
    background: #02457A;
    color: #ffffff;

    nav {
        display: flex;
        align-items: center;
        padding: 15px 16px;

        .branding {
            display: flex;
            align-items: center;
            gap: 8px;

            img {
                max-width: 35px;
            }

            h1 {
                font-size: 24px;
            }
        }

        .nav-routes {
            display: flex;
            flex: 1;
            justify-content: flex-end;
            gap: 12px;
            list-style: none;

            a {
                text-decoration: none;
                color: inherit;
            }
        }
    }
}
</style>