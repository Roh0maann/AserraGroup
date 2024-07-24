<template>
    <div class="bg-danger">
        <footer class="footer container">
            <div class="row py-5">
                <div class="col-xl-8 mb-4 mb-xl-0">
                    <div class="d-flex gap-2 mb-3 align-items-start">
                        <i class="fa-solid fa-location-dot mt-1"></i>
                        <a class="nav-link" href="#">
                            Office 8 Building, 20th Floor SCBD Lot 28<br />
                            Jl. Jend. Sudirman Kav 52-53, Jakarta 12190, Indonesia
                        </a>
                    </div>
                    <div class="d-flex gap-2 mb-3 align-items-center">
                        <i class="fa-solid fa-phone"></i>
                        <a class="nav-link" href="#">(021) 2933 3000</a>
                    </div>
                </div>

                <div class="col-xl-4 text-center text-xl-end">
                    <NuxtLink to="/">
                        <img src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/05/logo-aserra.png?fit=136%2C80&ssl=1"
                            alt="Aserra Group Logo" class="img-fluid logo-img w-50" />
                    </NuxtLink>
                </div>
            </div>

            <div
                class="d-flex flex-column flex-lg-row justify-content-between align-items-center border-top border-1 py-3">
                <ul class="navbar-nav d-flex flex-row mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link px-2" href="#">About</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link px-2" href="#">Careers</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link px-2" href="#">Businesses</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link px-2" href="#">Contact</a>
                    </li>
                </ul>
                <p class="m-0 text-center text-lg-end">
                    Copyright © 2023 Aserra Group. All Rights Reserved.
                </p>
            </div>
        </footer>
    </div>
</template>

<style scoped>
.footer .nav-link {
    color: black;
    transition: color 0.3s;
}

.footer .nav-link:hover {
    color: #ffb700;
}

.footer p {
    color: #a6a7a8;
}

.logo-img {
    max-width: 100%;
    height: auto;
}
</style>
