<template>
    <main>
        <section id="main-content">
            <div class="container">
                <h1>Content goes here</h1>
            </div>
        </section>

        <TabsSection />
    </main>
</template>

<script>
import TabsSection from './TabsSection.vue';

export default {
    name: 'MainContent',
    components: {
        TabsSection,
    }
}

</script>

<style lang="scss" scoped>
#main-content {
    background-color: #000;
    color: #fff;

    .container {
        padding: 50px 0;
    }
}
</style>