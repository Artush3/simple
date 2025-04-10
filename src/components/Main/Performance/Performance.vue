<template>
    <section class="section_performance">
        <div class="conteiner_content flex">
            <div class="section_performance_desc">
                <h1>Простые вещи. Из бумаги</h1>
                <p>Бума́га (предположительно от итал. bombagia, первоисточником же считается иранский) — волокнистый материал с минеральными добавками. </p>
                <a href="#"><button>Каталог</button></a>
            </div>
            <img id="first_img" src="../../../img/Main/Performance/Layer 2 copy.svg" alt="показ">
            <img id="second_img" src="../../../img/Main/Performance/Layer 2.svg" alt="показ">
            <img id="third_img" src="../../../img/Main/Performance/Layer 3.svg" alt="показ">
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
        display: none;
        position: relative;
        top: 30px;
    }
}

@media(max-width:768px) and (min-width:577px) {
    section.section_performance {
        div.section_performance_desc {
            max-width: 390px;
            
            h1 {
                font-size: 50px;
            }
        }

        img#second_img {
            display: inline-block;
        }
    }
}

@media(max-width:576px) {
    section.section_performance {
        div.section_performance_desc {
            max-width: 286px;

            h1 {
                font-size: 38px;
            }

            p {
                font-size: 16px;
            }

            a {
                button {
                    width: 196px;
                    height: 60px;
                }
            }
        }

        img#third_img {
            display: inline-block;
        }
    }
};

@media(min-width:769px) {
    section.section_performance {
        img#first_img {
            display: inline-block;
        }
    }
}
</style>