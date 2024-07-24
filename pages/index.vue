<template>
    <main>
        <div id="carouselExampleIndicators" class="carousel slide">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/05/hero.jpg?fit=1920%2C963&ssl=1"
                        class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/08/Coal-Mining-2-scaled.jpg?fit=2560%2C1440&ssl=1"
                        class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/05/hero-2.jpg?fit=1920%2C963&ssl=1"
                        class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/08/Rig-Maera-3-1.jpg?fit=1280%2C720&ssl=1"
                        class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/08/Nickel-Barge-5.webp?fit=1402%2C798&ssl=1"
                        class="d-block w-100" alt="...">
                </div>
            </div>

            <div class="carousel-caption">
                <div class="container position-relative">
                    <div class="row">
                        <div class="">
                            <NuxtLink to="/" class="nav-link text-center d-flex align-items-center p-0 m-0 gap-3"
                                id="logo">
                                <p class="p-0 m-0 align-items-center fs-5">ABOUT US</p><i
                                    class="fa-solid fa-circle-arrow-right fs-1 p-0 m-0"></i>
                            </NuxtLink>
                        </div>
                    </div>
                </div>
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0"
                        class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
                        aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
                        aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"
                        aria-label="Slide 4"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4"
                        aria-label="Slide 5"></button>
                </div>
            </div>

        </div>
    </main>
</template>

<style scope>
.carousel-caption {
    width: 70%;
    position: absolute;
    top: 72%;
    left: 43%;
    transform: translate(-50%, -50%);
    color: white;
    text-align: center;
}

.carousel-indicators [data-bs-target] {
    box-sizing: content-box;
    flex: 0 1 auto;
    width: 300px;
    height: 4px;
    padding: 0;
    margin-right: 3px;
    margin-left: 3px;
    text-indent: -999px;
    cursor: pointer;
    background-color: #fff;
    background-clip: padding-box;
    border: 0;
    border-top: 10px solid transparent;
    border-bottom: 10px solid transparent;
    opacity: .5;
    transition: opacity .6s ease;
}

.carousel-indicators {
    position: absolute;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 0;
    display: flex;
    justify-content: start;
    padding: 10px;
    margin-right: 0%;
    margin-bottom: 1rem;
    margin-left: 0%;
}

.carousel-indicators .active {
    opacity: 1;
    width: 300px;
}
</style>
