<template>
    <div class="weather">
        <div class="weather__top">
            <div class="weather__now">
                <div class="weather__data">
                    <p class="city__name">Toshkent</p>
                    <p class="now__date">28-February 15:46</p>
                    <span class="weather__gradus">6°C</span>
                </div>
                <div class="weather__img">
                    <img src="./styles/img/sunny.png" alt="sunny">
                    <p class="weather__status">Sunny</p>
                </div>
            </div>
            <div class="weather__citys">
                <p>Hududlar</p>
                <ul class="citys__lists">
                    <li class="city__list">
                        Toshkent shahri
                    </li>
                    <li class="city__list">
                        Andijon
                    </li>
                    <li class="city__list">
                        Namangan
                    </li>
                    <li class="city__list">
                        Farg'ona
                    </li>
                    <li class="city__list">
                        Sirdaryo
                    </li>
                    <li class="city__list">
                        Surxondaryo
                    </li>
                    <li class="city__list">
                        Qashqadaryo
                    </li>
                    <li class="city__list">
                        Xorazm
                    </li>
                    <li class="city__list">
                        Navoiy
                    </li>
                    <li class="city__list">
                        Buxoro
                    </li>
                    <li class="city__list">
                        Qoraqalpog'iston
                    </li>
                    <li class="city__list">
                        Toshkent vil
                    </li>
                </ul>
            </div>
        </div>
        <div class="weather__bottom">
            <div class="weather__hour">
                <h2>Soatlik prognoz:</h2>
                <ul class="weather__lists">
                    <li class="weather__list">
                        <p class="list__hour">18:00</p>
                        <img class="list__img" src="./styles/img/sunny.png" alt="">
                        <p class="list__gradus">26°C</p>
                    </li>
                    <li class="weather__list">
                        <p class="list__hour">18:00</p>
                        <img class="list__img" src="./styles/img/sunny.png" alt="">
                        <p class="list__gradus">26°C</p>
                    </li>
                    <li class="weather__list">
                        <p class="list__hour">18:00</p>
                        <img class="list__img" src="./styles/img/sunny.png" alt="">
                        <p class="list__gradus">26°C</p>
                    </li>
                    <li class="weather__list">
                        <p class="list__hour">18:00</p>
                        <img class="list__img" src="./styles/img/sunny.png" alt="">
                        <p class="list__gradus">26°C</p>
                    </li>
                    <li class="weather__list">
                        <p class="list__hour">18:00</p>
                        <img class="list__img" src="./styles/img/sunny.png" alt="">
                        <p class="list__gradus">26°C</p>
                    </li>
                </ul>
            </div>
            <div class="weather__5day">
                <p class="fday__title">5 kunlik prognoz:</p>
                <ul class="fday__lists">
                    <li class="fday__list">
                        <img src="./styles/img/rainy.png" alt="rain">
                        <p class="fday__gradus">18°C</p>
                        <p class="fday__data">Saturday, 2 Sep</p>
                    </li>
                    <li class="fday__list">
                        <img src="./styles/img/rainy.png" alt="rain">
                        <p class="fday__gradus">18°C</p>
                        <p class="fday__data">Saturday, 2 Sep</p>
                    </li>
                    <li class="fday__list">
                        <img src="./styles/img/rainy.png" alt="rain">
                        <p class="fday__gradus">18°C</p>
                        <p class="fday__data">Saturday, 2 Sep</p>
                    </li>
                    <li class="fday__list">
                        <img src="./styles/img/rainy.png" alt="rain">
                        <p class="fday__gradus">18°C</p>
                        <p class="fday__data">Saturday, 2 Sep</p>
                    </li>
                    <li class="fday__list">
                        <img src="./styles/img/rainy.png" alt="rain">
                        <p class="fday__gradus">18°C</p>
                        <p class="fday__data">Saturday, 2 Sep</p>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.weather {

    margin-top: 49px;
    width: 100%;

    // .weather__now

    &__now {
        display: flex;
        color: white;
        align-items: center;
        justify-content: space-around;
        background-color: rgb(68, 68, 68);
        border-radius: 30px;
        box-shadow: 10px 10px 5px rgb(0, 0, 0);
        padding: 0px 50px;
        gap: 20px;
        width: 100%;
    }

    &__data {
        margin-top: 30px;
    }

    // .weather__gradus

    &__gradus {
        font-family: Poppins;
        font-size: 90px;
        font-weight: 700;
    }

    // .weather__img

    &__img {
        img {
            width: 180px;
        }

        display: flex;
        flex-direction: column;
        text-align: center;
    }

    // .weather__status

    &__status {
        font-family: Poppins;
        font-size: 32px;
        font-weight: 600;
        padding-bottom: 10px;
    }

    // .weather__hour

    &__hour {}
}

.city {

    // .city__name

    &__name {
        font-size: 36px;
        font-family: Poppins;
        font-weight: 700;
        color: rgb(255, 255, 255);
    }
}

.now {

    // .now__date

    &__date {
        font-family: Poppins;
        font-size: 20px;
        font-weight: 400;
    }
}

.weather {

    // .weather__hour

    &__hour {
        width: 800px;
        height: 290px;
        border-radius: 30px;
        background: rgb(68, 68, 68);
        display: flex;
        flex-direction: column;
        margin-top: 30px;
        box-shadow: 10px 10px 5px rgb(0, 0, 0);

        h2 {
            font-family: Poppins;
            font-size: 32px;
            font-weight: 700;
            color: rgb(255, 255, 255);
            text-align: center;
            padding-top: 13px;
            margin-bottom: 10px;
        }
    }

    // .weather__lists

    &__lists {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 15px;
        height: 100%;
    }

    // .weather__list

    &__list {
        background-color: rgb(55, 54, 54);
        color: rgb(255, 255, 255);
        list-style-type: none;
        text-align: center;
        width: 15%;
        padding: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        gap: 12px;
        border-radius: 40px;
    }
}

.list {

    // .list__hour

    &__hour {
        font-family: Poppins;
        font-weight: 700;
        font-size: 24px;
    }

    // .list__img

    &__img {
        width: 80px;
    }

    // .list__gradus

    &__gradus {
        font-family: Poppins;
        font-weight: 700;
        font-size: 20px;
    }
}

.weather__top {
    display: flex;
    gap: 50px;
}

.weather {

    // .weather__citys

    &__citys {
        display: flex;
        flex-direction: column;

        p {
            font-family: Poppins;
            font-size: 33px;
            font-weight: 500;
            color: rgb(255, 255, 255);
            margin-bottom: 6px;
        }
    }
}

.citys {

    // .citys__lists

    &__lists {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
        cursor: pointer;
    }
}

.city {

    // .city__list

    &__list {
        list-style-type: none;
        color: #FFFFFF;
        font-family: Poppins;
        font-size: 16px;
        font-weight: 400;
        padding: 8px 24px;
        background-color: rgba(222, 226, 230, 0.2);
        border-radius: 6px;
    }
}

// 5 day weather 

.weather {

    &__bottom {
        display: flex;
        gap: 20px;
    }

    // .weather__5day

    &__5day {
        background-color: rgb(68, 68, 68);
        border-radius: 30px;
        width: 35%;
        box-shadow: 10px 10px 5px rgb(0, 0, 0);
    }
}

.fday {

    // .5day__lists

    &__lists {
        padding: 10px;
    }

    &__title {
        margin-top: 10px;
        text-align: center;
        font-family: Poppins;
        font-size: 32px;
        font-weight: 700;
        color: rgb(255, 255, 255);
    }

    // .5day__list

    &__list {
        display: flex;
        align-items: center;
        justify-content: space-around;
        gap: 30px;

        img {
            width: 50px;
        }
    }

    // .5day__gradus

    &__gradus {
        font-family: Poppins;
        font-size: 20px;
        font-weight: 500;
        color: rgb(255, 255, 255);
    }

    // .5day__data

    &__data {
        font-family: Poppins;
        font-size: 20px;
        font-weight: 500;
        color: rgb(255, 255, 255);
    }
}
</style>