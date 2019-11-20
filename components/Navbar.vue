<template>
    <div class="container">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <p class="navbar-brand">SomeBranD</p>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item ">
                        <nuxt-link exact class="nav-link" to="/">Главная</nuxt-link>
                    </li>
                    <li class="nav-item">
                        <nuxt-link active-class="active" class="nav-link" to="/about">О нас</nuxt-link>
                    </li>
                    <li class="nav-item">
                        <nuxt-link active-class="active" class="nav-link" to="/contact">Контакты</nuxt-link>
                    </li>
                </ul>
            </div>
        </nav>
    </div>
</template>