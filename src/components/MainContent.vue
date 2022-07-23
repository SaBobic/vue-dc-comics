<template>
    <main>
        <section id="main-content">
            <div class="container">
                <h1>Content goes here</h1>
            </div>
        </section>

        <section id="tabs" class="bg-primary">
        </section>
    </main>
</template>

<script>

export default {
    name: 'MainContent',
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

#tabs {
    color: #fff;
    height: 150px;
}
</style>