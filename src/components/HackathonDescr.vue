<template>
    <section class="hackathon-descr">
        <div class="container">
            <p class="descr">
                Уникальная возможность для разработчиков, дизайнеров и предпринимателей объединить свои усилия и создать
                инновационные технологические решения, которые могут изменить будущее.
            </p>
        </div>
    </section>
</template>

<style scoped>
.hackathon-descr {
    margin-bottom: 80px;
}

.descr {
    font-size: 28px;
    font-weight: 400;
    line-height: 33.6px;
    letter-spacing: 2%;
    color: #262626;
}

/* Adaptive */
@media screen and (max-width: 1175px) {
    .container {
        padding: 0 15px;
    }
}

@media screen and (max-width: 768px) {
    .hackathon-descr {
        margin-bottom: 40px;
    }
}

@media screen and (max-width: 590px) {
    .descr {
        font-size: 24px;
    }
}

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .descr {
        font-size: 20px;
    }

    .hackathon-descr {
        margin-bottom: 20px;
    }
}

@media screen and (max-width: 400px) {
    .descr {
        font-size: 16px;
    }
}
</style>