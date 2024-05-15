<script setup>
</script>
<template>
    <header>
        <div class="row">
            <nav class="navbar navbar-expand-sm">
                <a class="navbar-brand" href="#">
                    <img src="/src/assets/Exprerian/ProductPortalLogo.png">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mynavbar">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-end" id="mynavbar">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link login" href="#">Login</a>
                        </li>
                        <li class="nav-item">
                            <a class="btn btn-theme" href="#">Get Started  <i class="bi bi-arrow-up-right"></i></a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <h1 class="app-title">The Best and most Trusted<span> <br> <img class="app-pic" src="/src/assets/Exprerian/FinancialWording.png"></span> Products</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <img class="app-pic" src="/src/assets/Exprerian/Infographic1.png">
            </div>
        </div>
    </header>
</template>

<style>
    .login {
        text-decoration: none;
        margin-right: 1rem;
        align-self: center;
        color: #000;
    }
    .app-title{
        font: normal normal bold 70px/100px Roboto;
        text-align: center;
        letter-spacing: 0px;
        color: #19468D;
    }
    .app-pic {
        max-width: 100%;
    }
</style>