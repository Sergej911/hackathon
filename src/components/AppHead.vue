<template>
    <header class="header">
        <div class="container">
            <span class="logo">Логотип</span>
            <div class="header-content">
                <span class="date">
                    22-24 сентября 2022
                </span>
                <h1 class="header-title">
                    Agritech Innovathon 2022
                </h1>
                <ul class="about-list">
                    <li class="about-item">Coldstart</li>
                    <li class="about-item">ML</li>
                    <li class="about-item">RecSys</li>
                </ul>
                <div class="quantity">
                    <div class="participants">
                        <img src="/participants.svg" alt="">
                        <span>156</span>
                        <span>участников</span>
                    </div>
                    <div class="teams">
                        <img src="/teams.svg" alt="">
                        <span>23</span>
                        <span>команды</span>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
.logo {
    display: block;
    margin-bottom: 325px;
    font-family: 'Press Start 2P';
    font-size: 20px;
    font-weight: 400;
    line-height: 20px;
    color: #F9FAF9;
}

.header-content {
    display: flex;
    flex-direction: column;
    row-gap: 24px;
}

.header {
    margin-bottom: 80px;
    padding: 32px 0 94px 0;
    background-image: url('/public/hero.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.date {
    font-family: 'Press Start 2P';
    font-size: 32px;
    font-weight: 400;
    line-height: 35.2px;
    color: #C6D93B;
}

.header-title {
    font-family: 'Press Start 2P';
    font-size: 48px;
    font-weight: 400;
    line-height: 64px;
    color: #F9FAF9;
}

.about-list {
    display: flex;
    column-gap: 8px;
}

.about-item {
    padding: 8px 24px;
    font-size: 20px;
    font-weight: 500;
    line-height: 24px;
    color: #C6D93B;
    border: 2px solid #C6D93B;
    border-radius: 24px;
}

.quantity {
    display: flex;
    column-gap: 32px;
    align-items: center;
}

.participants,
.teams {
    display: flex;
    align-items: center;
    column-gap: 8px;
    font-size: 20px;
    font-weight: 500;
    line-height: 24px;
    color: #F9FAF9;
}

/* Adaptive */

@media screen and (max-width: 1175px) {
    .container {
        padding: 0 15px;
    }
}

@media screen and (max-width: 768px) {
    .header {
        margin-bottom: 40px;
    }

    .logo {
        margin-bottom: 200px;
    }
}

@media screen and (max-width: 524px) {
    .date {
        font-size: 26px;
    }

    .header-title {
        font-size: 42px;
    }
}

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .header {
        margin-bottom: 20px;
        padding: 25px 0 64px 0;
    }

    .logo {
        margin-bottom: 100px;
    }

    .header-title {
        font-size: 32px;
    }
}

@media screen and (max-width: 400px) {
    .about-list {
        flex-wrap: wrap;
        row-gap: 8px;
    }

    .quantity {
        flex-wrap: wrap;
    }

    .header-title {
        font-size: 28px;
    }
}
</style>