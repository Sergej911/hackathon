<template>
    <section class="hackathons">
        <div class="container">
            <div class="hackathons-head">
                <h2 class="title">Хакатоны</h2>
                <p class="section-descr">
                    Успей принять участие в хакатонах которые проходят прямо сейчас
                </p>
            </div>
            <ul class="hackathons-list">
                <li class="hackathons-item">
                    <div class="item-card">
                        <ul class="top-list">
                            <li>Сoldstart</li>
                            <li>ML</li>
                            <li>RecSys</li>
                        </ul>
                        <div class="item-bottom">
                            <span class="date">
                                15-17<br> июня
                            </span>
                            <a href="#">
                                <img class="link-img" src="/Button arrow.svg" alt="ссылка">
                            </a>
                        </div>
                    </div>
                    <div class="item-info">
                        <h3 class="info-title">
                            Tech Fishion Hackaton
                        </h3>
                        <p class="info-descr">
                            Уникальная возможность для разработчиков, дизайнеров и предпринимателей объединить свои
                            усилия и создать инновационные технологические решения, которые могут изменить будущее.
                        </p>
                    </div>
                </li>

                <li class="hackathons-item top">
                    <div class="item-card bg-2">
                        <ul class="top-list">
                            <li>NLP</li>
                            <li>ChatBots</li>
                            <li>Feedback</li>
                        </ul>
                        <div class="item-bottom">
                            <span class="date">
                                22-24<br> сентября
                            </span>
                            <a href="#">
                                <img class="link-img" src="/Button arrow.svg" alt="ссылка">
                            </a>
                        </div>
                    </div>
                    <div class="item-info">
                        <h3 class="info-title">
                            Tech Fishion Hackaton
                        </h3>
                        <p class="info-descr">
                            Уникальная возможность для разработчиков, дизайнеров и предпринимателей объединить свои
                            усилия и создать инновационные технологические решения, которые могут изменить будущее.
                        </p>
                    </div>
                </li>
            </ul>
            <div class="btn-wrap">
                <button class="btn">Смотреть все</button>
            </div>
        </div>
    </section>
</template>

<style scoped>
.hackathons {
    margin-bottom: 80px;
}

.hackathons-head {
    margin-bottom: 32px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.title {
    font-family: 'Press Start 2P';
    font-size: 48px;
    font-weight: 400;
    line-height: 56px;
    color: #262626;
}

.section-descr {
    text-align: right;
    max-width: 50%;
    font-size: 24px;
    font-weight: 500;
    line-height: 28px;
    color: #444444;
}

.hackathons-list {
    display: flex;
    justify-content: space-between;
}

.hackathons-item {
    max-width: 552px;
}

.top {
    margin-top: 80px;
    margin-bottom: 40px;
}

.hackathons-item .bg-2 {
    background-image: url('/hackathon-2.png');
}

.item-card {
    margin-bottom: 24px;
    display: flex;
    flex-direction: column;
    row-gap: 298px;
    border-radius: 16px;
    padding: 24px 20px;
    background-image: url('/hackathon-1.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.top-list {
    display: flex;
    column-gap: 8px;
}

.top-list li {
    padding: 8px 24px;
    border: 2px solid #C6D93B;
    color: #C6D93B;
    border-radius: 24px;
}

.date {
    font-family: 'Press Start 2P';
    font-size: 36px;
    font-weight: 400;
    line-height: 46.8px;
    color: #F9FAF9;
}

.link-img {
    border-radius: 50%;
    transition: all 0.2s;
}

.link-img:hover {
    /* transform: scale(1.1); */
    transform: translate(0, -5px);
    cursor: pointer;
    box-shadow: 0 5px 10px #262626;
}

.item-bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.info-title {
    margin-bottom: 16px;
    font-family: 'Press Start 2P';
    font-size: 24px;
    font-weight: 400;
    line-height: 31.2px;
    color: #262626;
}

.info-descr {
    font-size: 20px;
    font-weight: 500;
    line-height: 24px;
    letter-spacing: 2%;
    color: #444444;
}

.btn {
    display: block;
    margin: 0 auto;
    font-family: 'Raleway';
    padding: 16px 32px;
    font-size: 24px;
    font-weight: 600;
    line-height: 28px;
    color: #262626;
    border-radius: 32px;
    background-color: #C6D93B;
    transition: all 0.3s;
}

.btn:hover {
    background-color: #A6B92E;
}

.btn:active {
    background-color: #828C32;
}

/* Adaptive */
@media screen and (max-width: 1175px) {
    .container {
        padding: 0 15px;
    }

    .hackathons-item {
        max-width: 540px;
    }
}

@media screen and (max-width: 1136px) {
    .hackathons-item {
        max-width: 530px;
    }
}

@media screen and (max-width: 1116px) {
    .hackathons-item {
        max-width: 520px;
    }
}

@media screen and (max-width: 1100px) {
    .hackathons-item {
        max-width: 48%;

    }

    .date {
        font-size: 30px;
    }

    .hackathons-head {
        margin-bottom: 0px;
    }

    .title {
        font-size: 40px;
    }

    .section-descr {
        font-size: 22px;
    }
}

@media screen and (max-width: 856px) {
    .top-list {
        column-gap: 5px;
        font-size: 14px;
    }
}

@media screen and (max-width: 768px) {
    .title {
        font-size: 36px;
    }

    .top-list {
        display: flex;
        flex-wrap: wrap;
        row-gap: 5px;
    }

    .date {
        font-size: 26px;
    }

    .btn {
        font-size: 20px;
    }
}

@media screen and (max-width: 690px) {
    .item-bottom {
        flex-direction: column;
        align-items: flex-start;
    }

    .item-card {
        row-gap: 180px;
    }
}

@media screen and (max-width: 624px) {
    .section-descr {
        font-size: 20px;
    }

    .title {
        font-size: 32px;
    }
}

@media screen and (max-width: 590px) {
    .hackathons-list {
        flex-direction: column;
    }

    .hackathons-item {
        max-width: 100%;
    }

    .item-bottom {
        flex-direction: row;
        align-items: center;
    }

    .hackathons-head {
        flex-direction: column;
        align-items: flex-start;
    }

    .section-descr {
        max-width: 100%;
        text-align: left;
    }
}

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .hackathons {
        margin-bottom: 40px;
    }

    .hackathons-head {
        flex-direction: column;
    }

    .title {
        font-size: 32px;
    }

    .section-descr {
        max-width: 100%;
        text-align: left;
        font-size: 22px;
    }

    .hackathons-list {
        flex-direction: column;
    }

    .item-card {
        padding: 18px 14px;
    }

    .top-list {
        display: flex;
        flex-wrap: wrap;
        row-gap: 8px;
    }

    .top {
        margin-top: 40px;
    }

    .btn {
        padding: 12px 24px;
        font-size: 20px;
    }
}

@media screen and (max-width: 400px) {
    .title {
        font-size: 28px;
    }

    .section-descr {
        margin-bottom: 24px;
        font-size: 18px;
    }

    .info-descr {
        font-size: 18px;
    }
}
</style>