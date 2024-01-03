<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/icon-256-light.png" alt="">
                <h1> Vue Todo </h1>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">Home</RouterLink>
                <RouterLink to="/about">About</RouterLink>
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
    //background: linear-gradient(0deg, rgba(18, 61, 70, 1) 0%, rgba(22, 45, 55, 1) 64%, rgba(23, 39, 49, 1) 84%, rgba(25, 30, 41, 1) 100%);
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