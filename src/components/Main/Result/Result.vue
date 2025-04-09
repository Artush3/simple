<template>
    <section class="section_result">
        <div class="conteiner_content">
            <div class="section_result_examples">
                <div class="section_result_examples_analogy">
                    <img src="../../../img/Main/Result/Buissnes Cards v2 (85x55).svg" alt="пример №1">
                    <div class="section_result_examples_analogy_desc">
                        <h3>V.1</h3>
                        <p>Результат вашего обучения</p>
                    </div>
                </div>
                <div class="section_result_examples_analogy">
                    <img src="../../../img/Main/Result/Buissnes Cards v6 (85x55) 1.svg" alt="пример №2">
                    <div class="section_result_examples_analogy_desc">
                        <h3>V.2</h3>
                        <p>Результат вашего обучения</p>
                    </div>
                </div>
                <div class="section_result_examples_analogy">
                    <img src="../../../img/Main/Result/Buissnes Cards v5 (85x55) 1.svg" alt="пример №3">
                    <div class="section_result_examples_analogy_desc">
                        <h3>V.3</h3>
                        <p>Результат вашего обучения</p>
                    </div>
                </div>
            </div>
            <div class="section_result_white">
                <img src="../../../img/Main/Result/Folder v8 Open 1.svg" alt="пример белезны">
                <div class="section_result_white_desc">
                    <h1>Максимальная белизна</h1>
                    <p>Для повышения белизны, гладкости и мягкости в состав бумажной массы вводят белые минеральные вещества: мел, тальк, каолин и др. Эта операция называется наполнением.</p>
                    <p>Отлив бумажного листа осуществляют на бумагоделательной машине, важнейшей частью которой является непрерывно движущаяся (как транспортер) металлическая или капроновая сетка.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Result"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.section_result {
    @include main_block(90px, #EBEBEB);

    div.section_result_examples {
        @include flex(center, space-between);
        margin-bottom: 95px;

        div.section_result_examples_analogy {
            padding-top: 20px;
            border-top: 1px solid #C0C0C0;
            max-width: 350px;
            @include flex(center);

            div.section_result_examples_analogy_desc {
                margin-left: 30px;

                h3 {
                    @include text(18px, #666666, 150%, 500);
                }

                p {
                    @include text(18px, $line-height:150%);
                }
            }
        }
    }

    div.section_result_white {
        @include flex(center, space-between);

        div.section_result_white_desc {
            max-width: 350px;

            h1 {
                @include text(40px, #666666);
            }

            p {
                @include text(18px, $line-height:170%) {
                    margin-top: 15px;
                };
            }
        }
    }
}
</style>