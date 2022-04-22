<template>
    <div class="nav-bar">
    <div class="container">
        <nav class="nav__wrap">
            <div class="nav__left">
                <font-awesome-icon :icon="['fab', 'soundcloud']" class="nav__left-icon" />
                <span class="nav__left-title">
                    SOUND
                    <span class="nav__left-subtitle">BOX</span>
                </span>
            </div>
            <div class="nav__navigation">
                <ul class="nav__nav-list">
                    <li class="nav__nav-item">
                        <nuxt-link to="/">Home</nuxt-link>
                    </li>
                    <li class="nav__nav-item">
                        <nuxt-link to="/products">Products</nuxt-link>
                    </li>
                    <li class="nav__nav-item">
                        <nuxt-link to="/about">About us</nuxt-link>
                    </li>
                    <li class="nav__nav-item">
                        <nuxt-link to="/contact">Contact us</nuxt-link>
                    </li>
                </ul>
            </div>
            <div class="nav__right">
                <div class="nav__search">
                    <font-awesome-icon :icon="['fas', 'magnifying-glass']" class="nav__search-icon-search" />
                    <input type="text" placeholder="Search" class="nar__search-input">
                    <font-awesome-icon :icon="['fas', 'lock']" class="nav__search-icon-lock" />
                </div>
                <div class="nav__menu">
                    <font-awesome-icon :icon="['fas', 'bars']" class="nav__search-icon-menu" />
                </div>
            </div>
        </nav>
    </div>
    </div>
</template>
<style scoped>
    .nav-bar {
        background-color: black;
    }

    .nav__wrap {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 60px;
    }

    .nav__left-icon {
        color: #FFF;
        font-size: 3rem;
        margin-right: 5px;
    }

    .nav__left-title {
        color: #FFF;
        font-size: 1.8rem;
        font-weight: bold;
    }

    .nav__left-subtitle {
        color: #c7c7c7;
        font-weight: 400;
        margin-left: -5px;
    }

    .nav__navigation {
        display: flex;
    }

    .nav__nav-list {
        list-style: none;
        display: flex;
        margin: 0;
        padding: 0;
    }

    .nav__nav-item {
        padding: 0 20px;
    }

    .nav__nav-item a {
        text-decoration: none;
        color: #888;
        font-size: 1.5rem;
        font-weight: 500;
        padding: 10px;
    }

    .nav__nav-item a:hover {
        color: #FFF;
    }

    .nav__right {
        display: flex;
        justify-content: space-between;
        color: #888;
    }

    .nav__search {
        padding: 0 30px;
        position: relative;
        font-size: 1.6rem;
    }

    .nar__search-input {
        background-color: transparent;
        border: none;
        max-width: 80px;
        margin: 0 10px;
    }

    .nav__search-icon-lock {
        color: #FFF;
    }

    .nav__search::after {
        content: '';
        height: 100%;
        position: absolute;
        right: 0;
        border-right: solid 2px #303030;
    }

    .nav__menu {
        padding: 0 30px;
    }

    .nav__search-icon-menu {
        font-size: 2rem;
    }

</style>