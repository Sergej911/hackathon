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
</style>