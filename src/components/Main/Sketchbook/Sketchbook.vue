<template>
    <section class="section_sketchbook">
        <div class="conteiner_content flex">
            <div class="section_sketchbook_desc">
                <h1>Simple скетчбук</h1>
                <p>80 листов, твердая обложка, бумага  Fabriano 200 г/м2. Подойдет и для графики и для акварели. Для самых смелых творческих замыслов!</p>
                <a href="#"><button>Купить</button></a>
            </div>
            <img src="../../../img/Main/Sketchbook/pic.svg" alt="скетчбук">
        </div>
    </section>
</template>

<script>
export default {
    name: "Sketchbook"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.section_sketchbook {
    @include main_block(45px);

    div.section_sketchbook_desc {
        max-width: 350px;

        h1 {
            @include text(40px, #666666);
        }

        p {
            @include text(18px, $line-height:170%) {
                margin: 15px 0 25px;
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
        top: 45px;
    }
}
</style>