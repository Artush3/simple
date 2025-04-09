<template>
    <header class="header_content">
        <div class="conteiner_content flex">
            <img src="../../img/Header/Frame 85.svg" alt="логотип">
            <nav class="header_content_nav">
                <div class="header_content_nav_text-links">
                    <a href="#">Продукция</a>
                    <a href="#">Материалы</a>
                    <a href="#">О нас</a>
                    <a href="#">Контакты</a>
                </div>
                <div class="header_content_nav_img-links">
                    <a href="#"><img src="../../img/Header/search.svg" alt="поиск"></a>
                    <a href="#"><img src="../../img/Header/log_in.svg" alt="вход"></a>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
header.header_content {
    @include main_block(25px) {
        border-bottom: 1px solid #DDDDDD;
    };

    nav.header_content_nav {
        @include flex(center);

        div.header_content_nav_text-links {
            @include flex(center);
            margin-right: 60px;

            a {
                &:not(:last-of-type) {
                    margin-right: 60px;
                };
                @include text(20px, #4C5866);
            }
        }

        div.header_content_nav_img-links {
            @include flex(center);

            a {
                &:last-of-type {
                    margin-left: 30px;
                }
            }
        }
    }
}
</style>