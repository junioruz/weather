<template>
    <div class="header">
        <div class="header__inp">
            <img src="./styles/img/search.png" alt="search">
            <input type="text" placeholder="Shahar nomini kiriting ...">
        </div>
        <button class="header__btn">
            <img src="./styles/img/location.png" alt="Get Location">
            Joriy Joylashuv
        </button>
    </div>
</template>

<style lang="scss">
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 43px;

    // .header__inp

    &__inp {
        width: 60%;
        display: flex;
        align-items: center;
        padding-left: 25px;
        gap: 29px;
        background-color: rgb(68, 68, 68);
        border-radius: 20px;

        img {
            width: 35px;
            cursor: pointer;
        }

        input {
            width: 80%;
            padding: 14px;
            font: Poppins;
            font-weight: 500;
            font-size: 20px;
            Letter-spacing: 0%;
            text-align: left;
            color: rgba(255, 255, 255, 0.6);
            background-color: rgb(68, 68, 68);
            border: none;
            outline: none;
        }
    }

    // .header__btn

    &__btn {
        display: flex;
        align-items: center;
        gap: 5px;

        font: Poppins;
        font-size: 22px;
        font-weight: 800;
        color: rgba(255, 255, 255, 0.8);
        padding: 8px;
        background-color: rgb(76, 187, 23);
        border: none;
        border-radius: 16px;
        cursor: pointer;

        img {
            width: 30px;
        }
    }
}
</style>