<template>
    <section class="results">
        <div class="container">
            <div class="results-content">
                <h2 class="title">Результаты</h2>
                <ul class="results-list">
                    <li v-for="item in results" :key="item.id" class="results-item">
                        <span class="number">{{ formatNumber(item.number) }}</span>
                        <div class="results-info">
                            <h3 class="results-title">{{ item.title }}</h3>
                            <p class="results-descr">
                                {{ isExpanded[item.id] ? item.descr : truncateText(item.descr, 200) }}
                            </p>
                            <div class="results-buttons">
                                <button @click="toggleExpand(item.id)" class="btn-1 btn">
                                    {{ isExpanded[item.id] ? 'Скрыть' : 'Читать полностью' }}
                                </button>
                                <button class="btn-2 btn">Презентация</button>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

const results = ref([
    {
        id: 1,
        number: '1',
        title: 'AgriGigital',
        descr: 'Команда AgriDigital разработала комплексное решение для цифровизации фермерских хозяйств. Их система включает в себя интегрированные модули для мониторинга состояния почвы, посевов и животных, сбора и анализа данных, а также автоматизированного управления различными процессами на ферме. Решение отличается высокой точностью, гибкостью и простотой в использовании, что позволяет фермерам повысить эффективность и прибыльность своего бизнеса.'
    },
    {
        id: 2,
        number: '2',
        title: 'CropOptimizer',
        descr: 'Команда CropOptimizer  представила инновационное решение, сочетающее мобильное приложение и облачную платформу для цифровизации фермерских хозяйств. Их система собирает и анализирует данные о погодных условиях, состоянии почвы и растений, позволяя фермерам оптимизировать сроки и режимы полива, внесения удобрений и других агротехнических мероприятий. Решение отличается высокой точностью прогнозов и простотой интеграции с существующими системами на ферме.'
    },
    {
        id: 3,
        number: '3',
        title: 'FarmSense',
        descr: 'Команда FarmSense разработала комплексную систему бизнес-аналитики для фермерских хозяйств. Их решение включает в себя сбор и визуализацию данных о производственных показателях, финансах, логистике и других ключевых аспектах деятельности фермы. Система позволяет выявлять закономерности, оптимизировать бизнес-процессы и принимать обоснованные управленческие решения, что способствует повышению эффективности и рентабельности фермерского бизнеса.'
    },
])

const isExpanded = ref({});

const truncateText = (text, maxLength) => {
    return text.length > maxLength ? text.slice(0, maxLength) + '...' : text
}

const toggleExpand = (id) => {
    isExpanded.value[id] = !isExpanded.value[id]
}


const formatNumber = (number) => {
    return number.toString().padStart(2, '0')
}
</script>

<style scoped>
.results {
    margin-bottom: 24px;
}

.results-content {
    padding: 0 24px;
}

.title {
    font-family: 'Press Start 2P';
    font-size: 36px;
    font-weight: 400;
    line-height: 43.2px;
    color: #262626;
}

.results-item {
    padding: 24px 20px;
    display: flex;
    column-gap: 56px;
}

.number {
    font-family: 'Press Start 2P';
    font-size: 40px;
    font-weight: 400;
    line-height: 48px;
    color: #828C32;
}

.results-title {
    margin-bottom: 16px;
    font-family: 'Press Start 2P';
    font-size: 40px;
    font-weight: 400;
    line-height: 48px;
    color: #262626;
}

.results-descr {
    margin-bottom: 16px;
    font-size: 24px;
    font-weight: 400;
    line-height: 28px;
    letter-spacing: 2%;
    color: #444444;
}

.results-buttons {
    display: flex;
    column-gap: 16px;
}

.btn-1 {
    padding: 16px 32px;
    border-radius: 32px;
    background-color: #C6D93B;
    font-size: 24px;
    font-weight: 400;
    line-height: 28px;
    letter-spacing: 2%;
    font-family: 'Raleway';
    cursor: pointer;
    transition: all 0.3s;
}

.btn-1:hover {
    background-color: #A6B92E;
}

.btn-1:active {
    background-color: #828C32;
}

.btn-2 {
    padding: 16px 32px;
    border: 2px solid #262626;
    border-radius: 32px;
    background: none;
    font-size: 24px;
    font-weight: 400;
    line-height: 28px;
    letter-spacing: 2%;
    cursor: pointer;
    font-family: 'Raleway';
    transition: all 0.3s;
}

.btn-2:hover {
    color: #fff;
    background-color: #262626;
}

.btn-2:active {
    background-color: #262626b2;
}

/* Adaptive */

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .results-content {
        padding: 0;
    }

    .results-item {
        padding: 20px 0;
        flex-direction: column;
    }

    .title {
        margin-bottom: 0;
        font-size: 28px;
    }

    .results-title {
        font-size: 24px;
        margin-bottom: 6px;
    }

    .number {
        margin-bottom: 0;
        font-size: 28px;
        margin-left: 10px;
    }

    .results-descr {
        font-size: 20px;
    }

    .btn {
        padding: 8px 22px;
        font-size: 20px;
    }
}
</style>