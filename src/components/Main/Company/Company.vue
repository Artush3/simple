<template>
    <section class="section_company">
        <div class="conteiner_content flex">
            <div class="section_company_partner">
                <img src="../../../img/Main/Company/hahnemuehle-logo-vector 1.svg" alt="компания №1">
            </div>
            <div class="section_company_partner">
                <img src="../../../img/Main/Company/Frame 225.svg" alt="компания №2">
            </div>
            <div class="section_company_partner">
                <img src="../../../img/Main/Company/royal-talens-bv-logo-vector 1.svg" alt="компания №3">
            </div>
            <div class="section_company_partner">
                <img src="../../../img/Main/Company/Frame.svg" alt="компания №4">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Company"
}
</script>

<style scoped lang="scss">
@use "../../../assets/mixins.scss" as *;
section.section_company {
    @include main_block(90px, #EBEBEB);

    div.section_company_partner {
        height: 135px;
        width: 255px;
        @include flex(center, center);
        border:  1px solid #C4C4C4;
    }
}
</style>