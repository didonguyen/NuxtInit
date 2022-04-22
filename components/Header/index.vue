<template>
    <div class="header">
        <div class="header__content">
            <div class="header__content-color-title">
                Over-Ear Stereo
            </div>
            <div class="header__content-title">
                Experience Media <br> Like Never Before
            </div>
            <div class="header__content-subtitle">
                The best product for your life. Come to see us and buy anything. <br> Purchase anything with 20% discount.
            </div>
            <div class="header__content-action">
                <div class="header__content-action-left">
                    <button class="header__content-action-button">SEE MORE</button>
                </div>
                <div class="header__content-action-right">
                    <font-awesome-icon :icon="['fas', 'circle-play']" class="header__content-button-icon"/>
                    <span class="header__content-button-content">Watch Video</span>
                </div>
            </div>
            <div class="header__content-socials">
                <font-awesome-icon :icon="['fab', 'facebook-f']" class="header__content-socials-icon" />
                <font-awesome-icon icon="fa-brands fa-twitter" class="header__content-socials-icon" />
                <font-awesome-icon icon="fa-brands fa-instagram" class="header__content-socials-icon" />
            </div>
        </div>
        <div class="header__img">
            <img src="~/assets/img/headphone-1.png" alt="headphone" class="header__img-image">
        </div>
    </div>
</template>
<style scoped>
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 30px;
    }

    .header__content {
        width: 50%;
    }

    .header__content-color-title {
        background: -webkit-linear-gradient(#2EE0E6, #EC79FD);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-size: 2.5rem;
        font-weight: 500;
    }

    .header__content-title {
        color: #FFF;
        font-size: 5.5rem;
        font-weight: 500;
        margin-top: 30px;
    }

    .header__content-subtitle {
        color: #666;
        font-size: 1.6rem;
        font-weight: 500;
        margin-top: 30px;
    }

    .header__content-action {
        margin-top: 60px;
        display: flex;
    }

    .header__content-action-button {
        background-image: linear-gradient(to right, #3f9afc, #5d97ff, #7693ff, #8e8eff, #a488fd);
        border: none;
        border-radius: 3px;
        padding: 14px 20px;
        color: #FFF;
        font-weight: 500;
        min-width: 150px;
        letter-spacing: 2px;
    }

    .header__content-action-right {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-left: 40px;
    }

    .header__content-button-icon {
        font-size: 3rem;
        color: #FFF;
        position: relative;
    }

    .header__content-button-icon::after {
        content: '';
        position: absolute;
        width: 50px;
        height: 50px;
        top: 0;
        background-color: #FFF;
    }

    .header__content-button-content {
        color: #9c9c9c;
        font-size: 1.4rem;
        font-weight: 500;
        margin-left: 15px;
    }

    .header__content-socials-icon {
        color: #FFF;
        font-size: 1.6rem;
    }

    .header__img {
    }

    .header__img-image {
        width: 80%;
    }

</style>