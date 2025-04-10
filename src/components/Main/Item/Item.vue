<template>
    <section class="section_item">
        <div class="conteiner_content">
            <div class="section_item_product">
                <img id="first_img" src="../../../img/Main/Item/Frame 208.svg" alt="продукт №1">
                <img id="second_img" src="../../../img/Main/Item/Frame 2081.svg" alt="продукт №1">
                <h2>Упаковка</h2>
                <h3>Тираж: от 50 штук</h3>
                <p>Сделано из крафт-бумаги или плотного картона. Упаковки имеют различные формы и расцветки, изготовим форму под заказ.</p>
                <a href="#">
                    <p>Подробнее</p>
                    <img src="../../../img/Main/Item/Arrow 1.svg" alt="подробнее">
                </a>
            </div>
            <div class="section_item_product">
                <img id="first_img" src="../../../img/Main/Item/Frame 209.svg" alt="продукт №2">
                <img id="second_img" src="../../../img/Main/Item/Frame 2091.svg" alt="продукт №2">
                <h2>Пакеты</h2>
                <h3>Тираж: от 200 штук</h3>
                <p>С прямоугольным дном. От 10 см до 60 см по высоте. Материалы: картон, крафт-бумага. Различные расцветки и дизайн.</p>
                <a href="#">
                    <p>Подробнее</p>
                    <img src="../../../img/Main/Item/Arrow 1.svg" alt="подробнее">
                </a>
            </div>
            <div class="section_item_product">
                <img id="first_img" src="../../../img/Main/Item/Frame 211.svg" alt="продукт №3">
                <img id="second_img" src="../../../img/Main/Item/Frame 2111.svg" alt="продукт №3">
                <h2>Кейсы</h2>
                <h3>Тираж: от 30 штук</h3>
                <p>Подойдет для документов и других бумаг. Различные расцветки, размеры и плотность. Материал: прессованная бумага.</p>
                <a href="#">
                    <p>Подробнее</p>
                    <img src="../../../img/Main/Item/Arrow 1.svg" alt="подробнее">
                </a>
            </div>
            <div class="section_item_product">
                <img id="first_img" src="../../../img/Main/Item/Frame 210.svg" alt="продукт №4">
                <img id="second_img" src="../../../img/Main/Item/Frame 2101.svg" alt="продукт №4">
                <h2>Другие изделия </h2>
                <h3>Тираж: от 100 штук</h3>
                <p>Нестандартные упаковки, кейсы и другие изделия различных размеров и конфигураций. Изготовим в кратчайшие сроки.</p>
                <a href="#">
                    <p>Подробнее</p>
                    <img src="../../../img/Main/Item/Arrow 1.svg" alt="подробнее">
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Item"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.section_item {
    @include main_block(80px);

    div.conteiner_content {
        @include flex(start, space-between);

        div.section_item_product {
            max-width: 255px;

            > img {
                display: none;
                width: 100%;
            }

            h2 {
                @include text(30px, #666666) {
                    margin: 20px 0 10px;
                };
            }

            h3 {
                @include text(14px, #B5B5BD);
            }

            > p {
                @include text(18px, $line-height:170%) {
                    margin: 10px 0 20px;
                };
            }

            a {
                @include flex(center);
                width: max-content;

                p {
                    @include text(20px, #7875FE) {
                        margin-right: 5px;
                    };
                }
            }
        }
    }
}

@media(max-width:768px) {
    section.section_item {
        @include main_block(50px);

        div.conteiner_content {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            grid-column-gap: 30px;
            grid-row-gap: 50px;

            div.section_item_product {
                max-width: 100%;

                img#second_img {
                    display: inline-block;
                }
            }
        }
    }
}

@media(min-width:769px) {
    section.section_item {
        div.section_item_product {
            img#first_img {
                display: inline-block;
            }
        }
    }
}

@media(max-width:320px) {
    section.section_item {
        div.conteiner_content {
            grid-template-columns: 1fr;
        }
    }
}
</style>