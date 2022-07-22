<template>
    <header id="main-header">
        <nav class="container">
            <figure>
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="DC Comics Logo">
                </a>
            </figure>

            <ul>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#" class="active">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
                <li>
                    <a href="#">VIDEO</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>

export default {
    name: 'MainHeader',
}

</script>

<style scoped>
#main-header nav {
    padding: 20px 0;
}

#main-header nav,
#main-header ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#main-header img {
    height: 80px;
}

#main-header ul {
    font-size: 12px;
    font-weight: 700;
}

#main-header ul li {
    margin: 0 15px;
}

#main-header ul li a {
    padding: 100% 0;
    position: relative;
}

#main-header ul li a.active,
#main-header ul li a:hover {
    color: #0282F9;
}

#main-header ul li a:hover::after,
#main-header ul li a.active::after {
    content: '';
    width: 100%;
    height: 6px;
    background-color: #0282F9;
    position: absolute;
    bottom: -18px;
    left: 0;
}
</style>