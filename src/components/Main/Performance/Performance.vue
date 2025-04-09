<template>
    <section class="section_performance">
        <div class="conteiner_content flex">
            <div class="section_performance_desc">
                <h1>Простые вещи. Из бумаги</h1>
                <p>Бума́га (предположительно от итал. bombagia, первоисточником же считается иранский) — волокнистый материал с минеральными добавками. </p>
                <a href="#"><button>Каталог</button></a>
            </div>
            <img src="../../../img/Main/Performance/Layer 2 copy.svg" alt="показ">
        </div>
    </section>
</template>

<script>
export default {
    name: "Performance"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.section_performance {
    @include main_block(30px);

    div.section_performance_desc {
        max-width: 445px;

        h1 {
            @include text(60px, #4C5866);
        }

        p {
            @include text(18px, $line-height:150%) {
                margin: 30px 0;
            };
        }

        a {
            button {
                @include button;
            }
        }
    }

    img {
        position: relative;
        top: 30px;
    }
}
</style>