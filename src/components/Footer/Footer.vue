<template>
    <footer class="section_header">
        <section class="section_header_nav">
            <div class="conteiner_content flex">
                <img src="../../img/Footer/Frame 85 (1).svg" alt="логотип">
                <nav class="section_header_nav_way">
                    <a href="#"><img src="../../img/Footer/Frame (1).svg" alt="Facabook"></a>
                    <a href="#"><img src="../../img/Footer/Frame (2).svg" alt="Twitter"></a>
                    <a href="#"><img src="../../img/Footer/Frame (3).svg" alt="Instagram"></a>
                    <a href="#"><img src="../../img/Footer/Frame (4).svg" alt="YouTube"></a>
                </nav>
            </div>
        </section>
        <section class="section_header_date">
            <h2>SIMPLE ® 2025</h2>
        </section>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
section.section_header_nav {
    @include main_block(25px, #4C5866);

    nav.section_header_nav_way {
        a {
            &:not(:last-of-type) {
                margin-right: 30px;
            }
        }
    }
}

section.section_header_date {
    @include flex(center, center);

    h2 {
        @include text(13px, black);
    }
}
</style>