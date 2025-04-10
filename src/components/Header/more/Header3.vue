<template>
    <header class="header3_content">
        <section class="header3_content_logo">
            <img src="../../../img/Header/Frame 85.svg" alt="логотип">
        </section>
        <section class="header3_content_nav">
            <div class="conteiner_content flex">
                <img @click="showMenu" src="../../../img/Header/List.svg" alt="меню">
                <nav class="header3_content_menu-links">
                    <a href="#"><img src="../../../img/Header/search.svg" alt="поиск"></a>
                    <a href="#"><img src="../../../img/Header/log_in.svg" alt="вход"></a>
                </nav>
            </div>
        </section>
        <section v-if="menu" class="header3_content_menu">
            <div class="conteiner_content">
                <img @click="showMenu" src="../../../img/Header/Frame 7.svg" alt="менню">
                <a href="#">Продукция</a>
                <a href="#">Материалы</a>
                <a href="#">О нас</a>
                <a href="#">Контакты</a>
            </div>
        </section>
    </header>
</template>

<script>
export default {
    name: "Header3",
    data() {
        return {
            menu: false
        }
    },
    methods: {
        showMenu() {
            this.menu = !this.menu
        }
    }
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.header3_content_logo {
    @include main_block(10px) {
        border-bottom: 1px solid #DDDDDD;
    };
    @include flex(center, center);
}

section.header3_content_nav {
    @include main_block(15px) {
        border-bottom: 1px solid #DDDDDD;
    };

    img {
        &:first-of-type {
            cursor: pointer;
        }
    }

    nav.header3_content_menu-links {
        a {
            &:last-of-type {
                margin-left: 25px;
            }
        }
    }
}

section.header3_content_menu {
    padding-top: 15px;
    position: absolute;
    height: 400px;
    width: 100%;
    background-color: #EBEBEB;
    top: 43px;

    img {
        &:first-of-type {
            cursor: pointer;
        }
    }

    a {
        display: block;
        @include text(18px, #4C5866);
        margin-top: 50px;
    }
}

@media(min-width:321px) {
    header.header3_content {
        display: none;
    }
}
</style>