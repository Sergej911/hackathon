<template>
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-left">
                    <p class="logo bold">Логотип</p>
                    <p class="copyright">© 2024. Все права защищены. </p>
                </div>

                <div class="footer-right">
                    <span class="bold contacts">Контакты</span>
                    <a href="mailto:cnois_hakaton@mail.ru">Email: cnois_hakaton@mail.ru</a>
                    <a href="tel:+70000000000">Телефон: +7 (000) 000-00-00</a>
                    <a href="https://www.instagram.com/cnois_hakaton" target="_blank">Inst: @cnois_hakaton</a>
                    <a href="https://vk.com/cnois_hakaton" target="_blank">vk: https://vk.com/cnois_hakaton</a>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer {
    margin-bottom: 32px;
}

.footer-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    margin-bottom: 8px;
}

.footer-right {
    display: flex;
    flex-direction: column;
    row-gap: 8px;
    text-align: right;
}

.contacts {
    margin-bottom: 4px;
}

.bold {
    display: block;
    font-family: 'Press Start 2P';
    font-weight: 400;
    font-size: 20px;
    line-height: 20px;
    color: #262626;
}

.copyright {
    font-size: 16px;
    font-weight: 500;
    line-height: 19.2px;
    letter-spacing: 2%;
    color: #383849;
}

a {
    font-size: 16px;
    font-weight: 500;
    line-height: 19.2px;
    letter-spacing: 2%;
    color: #383849;
    transition: all 0.2s;
}

a:hover {
    color: #38384998;
}

a:active {
    color: #3838499c;
}

/* Adaptive */

@media screen and (max-width: 480px) {
    .container {
        padding: 0 15px;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }

    .footer-left {
        margin-bottom: 16px;
    }

    .footer-right {
        text-align: center;
    }
}
</style>