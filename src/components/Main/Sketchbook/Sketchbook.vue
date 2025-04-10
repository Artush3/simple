<template>
    <section class="section_sketchbook">
        <div class="conteiner_content flex">
            <img id="third_img" src="../../../img/Main/Sketchbook/pic3.svg" alt="скетчбук">
            <div class="section_sketchbook_desc">
                <h1>Simple скетчбук</h1>
                <p>80 листов, твердая обложка, бумага  Fabriano 200 г/м2. Подойдет и для графики и для акварели. Для самых смелых творческих замыслов!</p>
                <a href="#"><button>Купить</button></a>
            </div>
            <img id="first_img" src="../../../img/Main/Sketchbook/pic.svg" alt="скетчбук">
            <img id="second_img" src="../../../img/Main/Sketchbook/pic1.svg" alt="скетчбук">
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
        display: none;
        position: relative;
        top: 45px;
    }
}

@media(max-width:768px) and (min-width:577px) {
    section.section_sketchbook {
        @include main_block(30px);

        div.section_sketchbook_desc {
            max-width: 330px;
            
            h1 {
                font-size: 30px;
            }
        }

        img#second_img {
            display: inline-block;
            position: relative;
            left: 30px;
            top: 30px;
        }
    }
}

@media(min-width:769px) {
    section.section_sketchbook {
        img#first_img {
            display: inline-block;
        }
    }
}

@media(max-width:576px) {
    section.section_sketchbook {
        div.conteiner_content {
            display: block;
            div.section_sketchbook_desc {
                max-width: 100%;
                
                h1 {
                    font-size: 24px;
                }

                p {
                    font-size: 16px;
                }

                a {
                    button {
                        height: 60px;
                        width: 196px;
                    }
                }
            }

            img#third_img {
                display: inline-block;
                margin-bottom: 50px;
            }
        }
    }
}
</style>