<template>
    <header class="header2_content">
        <section class="header2_content_cover">
            <div class="conteiner_content flex">
                <img src="../../../img/Header/Frame 85.svg" alt="логотип">
                <nav class="header2_content_cover_img-links">
                    <a href="#"><img src="../../../img/Header/search.svg" alt="поиск"></a>
                    <a href="#"><img src="../../../img/Header/log_in.svg" alt="вход"></a>
                </nav>
            </div>
        </section>
        <section class="eader2_content_way">
            <div class="conteiner_content flex">
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
    name: "Header2"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.header2_content_cover {
    @include main_block(10px) {
        border-bottom: 1px solid #DDDDDD;
    };

    nav.header2_content_cover_img-links {
        a {
            img {
                &:last-of-type {
                    margin-left: 25px;
                }
            }
        }
    }
}

section.eader2_content_way {
    @include main_block(20px) {
        border-bottom: 1px solid #DDDDDD;
    };

    a {
        @include text(20px, #4C5866);
    }
}

@media(min-width:769px) {
    header.header2_content {
        display: none;
    }
}
</style>