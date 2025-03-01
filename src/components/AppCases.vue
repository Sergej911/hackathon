<template>
    <section class="cases">
        <div class="container">
            <div class="cases-head">
                <h2 class="title">Кейсы</h2>
                <p class="section-descr">
                    Список ситуаций, проблем или задач, которые необходимо проанализировать
                </p>
            </div>
            <ul class="cases-list">
                <li class="cases-item-1 case">
                    <ul class="case-top">
                        <li>Сенсорные технологии</li>
                        <li>Робототехника</li>
                        <li>Анализ данных</li>
                    </ul>
                    <h3 class="cases-title">Точное земледелие</h3>
                </li>

                <li class="cases-item-2 case">
                    <ul class="case-top">
                        <li class="top-white">Большие данные</li>
                        <li class="top-white">Мобильные приложения</li>
                        <li class="top-white">Бизнес-аналитика</li>
                    </ul>
                    <h3 class="white cases-title">Цифровая ферма</h3>
                    <p class="cases-descr">
                        Разработка комплексных решений для цифровизации фермерских хозяйств, включая
                        системы мониторинга,
                        управления и анализа данных.
                    </p>
                </li>

                <app-results />

                <li class="cases-item-3 case">
                    <ul class="case-top">
                        <li class="top-white">Компьютерная графика</li>
                        <li class="top-white">Мобильная разработка</li>
                        <li class="top-white">UX/UI</li>
                    </ul>
                    <h3 class="cases-title title-3">Виртуальная примерочная</h3>
                </li>

                <li class="cases-item-4 case">
                    <ul class="case-top">
                        <li class="top-green">Робототехника</li>
                        <li class="top-green">Программирование</li>
                        <li class="top-green">Бизнес-аналитика</li>
                    </ul>
                    <h3 class="cases-title title-4">Инновации в производстве</h3>
                </li>
            </ul>
        </div>
    </section>
</template>

<script setup>
import AppResults from "./AppResults.vue";
</script>

<style scoped>
.cases {
    margin-bottom: 80px;
}

.cases-head {
    margin-bottom: 32px;
    display: flex;
    justify-content: space-between;
}

.title {
    font-family: 'Press Start 2P';
    font-size: 48px;
    font-weight: 400;
    line-height: 57.6px;
    color: #262626;
}

.section-descr {
    max-width: 45%;
    font-size: 24px;
    font-weight: 500;
    line-height: 28.8px;
    text-align: right;
    color: #444444;
}

.cases-item-1 {
    margin-bottom: 24px;
    background-color: #C6D93B;
}

.cases-item-2 {
    margin-bottom: 32px;
    background-color: #828C32;
}

.cases-item-3 {
    margin-bottom: 24px;
    background-color: #3E402D;
}

.cases-item-4 {
    background-color: #262626;
}

.case .title-3 {
    color: #F9FAF9;
}

.case .title-4 {
    color: #C6D93B;
}

.case-top .top-green {
    color: #C6D93B;
    border-color: #C6D93B;
}

.case {
    padding: 24px 20px;
    border-radius: 16px;
}

.case-top {
    margin-bottom: 48px;
    display: flex;
    column-gap: 8px;
}

.case-top li {
    padding: 8px 24px;
    border: 2px solid #262626;
    border-radius: 24px;
    font-size: 20px;
    font-weight: 500;
    line-height: 24px;
    letter-spacing: 2%;
    color: #262626;
}

.cases-title {
    font-family: 'Press Start 2P';
    font-size: 24px;
    font-weight: 400;
    line-height: 28px;
    color: #262626;
}

.white {
    margin-bottom: 16px;
    color: #F9FAF9;
}

.case-top .top-white {
    color: #F9FAF9;
    border-color: #F9FAF9;
}

.cases-descr {
    font-size: 24px;
    font-weight: 400;
    line-height: 28px;
    color: #fff;
}

/* Adaptive */
@media screen and (max-width: 1175px) {
    .container {
        padding: 0 15px;
    }
}

@media screen and (max-width: 852px) {
    .section-descr {
        max-width: 60%;
        font-size: 22px;
    }

    .cases-head {
        margin-bottom: 20px;
    }
}

@media screen and (max-width: 768px) {
    .cases-head {
        flex-direction: column;
    }

    .section-descr {
        max-width: 100%;
        text-align: left;
    }

    .title {
        font-size: 36px;
    }
}

@media screen and (max-width: 700px) {
    .case-top {
        flex-wrap: wrap;
        row-gap: 8px;
    }
}

@media screen and (max-width: 590px) {
    .case-top li {
        font-size: 18px;
    }

    .cases-descr {
        font-size: 20px;
    }

    .cases-title {
        font-size: 22px;
    }
}

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .cases {
        margin-bottom: 40px;
    }

    .cases-head {
        flex-direction: column;
        row-gap: 10px;
    }

    .title {
        font-size: 28px;
    }

    .section-descr {
        max-width: 100%;
        text-align: left;
        font-size: 20px;
    }

    .case-top {
        flex-wrap: wrap;
        row-gap: 10px;
    }

    .cases-title {
        font-size: 20px;
    }

    .cases-descr {
        font-size: 20px;
    }
}
</style>