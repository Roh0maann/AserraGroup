<template>
    <nav class="navbar navbar-expand-lg fixed-top custom-nav">
        <div class="container wraper-logo"> 
            <NuxtLink to="/" class="logo-container" id="logo">
                <img id="logo" class="p-0 m-0" width="136" height="80"
                    src="https://i0.wp.com/aserragroup.com/wp-content/uploads/2023/05/logo-aserra.png?fit=136%2C80&ssl=1"
                    alt="Aserra Group Logo" />
            </NuxtLink>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="ms-auto p-0" id="navbarNav">
                <ul class="navbar-nav flex-row">
                    <li class="nav-item menu-item">
                        <a class="nav-link text-white" href="#">HOME</a>
                    </li>
                    <li class="nav-item menu-item">
                        <a class="nav-link text-white" href="#">ABOUT</a>
                    </li>
                    <li class="nav-item menu-item">
                        <a class="nav-link text-white" href="#">BUSINESSES</a>
                    </li>
                    <li class="nav-item menu-item">
                        <a class="nav-link text-white" href="#">CAREERS</a>
                    </li>
                    <li class="nav-item menu-item">
                        <a class="nav-link text-white" href="#">CONTACT</a>
                    </li>
                    <button class="navbar-toggler offcanvas-toggler" type="button" data-bs-toggle="offcanvas"
                        data-bs-target="#navbarOffcanvasLg" aria-controls="navbarOffcanvasLg">
                        <span class="navbar-toggler-icon text-white"></span>
                    </button>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Offcanvas Navbar -->
    <div class="offcanvas offcanvas-end" tabindex="-1" id="navbarOffcanvasLg" aria-labelledby="offcanvasNavbarLabel">
        <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasNavbarLabel">Menu</h5>
            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link" href="#">HOME</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">ABOUT</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">BUSINESSES</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">CAREERS</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">CONTACT</a>
                </li>
            </ul>
        </div>
    </div>
</template>


<style scoped>
@media (max-width: 991px) {
    .offcanvas-toggler {
        display: none;
    }
}

@media (min-width: 992px) {
    .navbar-nav {
        display: flex;
        align-items: center;
    }

    .offcanvas-toggler {
        display: inline-block;
    }
}

.logo-container {
    transition: 0.3s;
    display: inline-block;
    width: 100%; 
    max-width: 134px;
    padding: 0px 0;
}

.custom-nav {
    background: linear-gradient(180deg, #171717 0%, rgba(23, 23, 23, 0) 100%);
    padding: 25px 0;
    transition: background 0.3s ease, padding 0.3s ease;
}

.navbar-scroll {
    padding: 0px 0;
    /* Reduced padding on scroll */
}

.navbar-toggler {
    padding: 0;
    font-size: var(--bs-navbar-toggler-font-size);
    line-height: 1;
    color: white;
    background-color: transparent;
    border: none;
}

.navbar-toggler:focus,
.navbar-toggler:active {
    outline: none;
    box-shadow: none;
}

#logo {
    transition: transform 0.3s ease, max-width 0.3s ease;
    max-width: 136px;
    /* Ensure logo doesn’t exceed its original size */
}

.logo-small {
    padding: 0px 0;
    transform: scale(0.60);
    /* Scale down */
    max-width: 100px;
    /* Reduce size when scrolled */
}
</style>

<script>
export default {
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            const navbar = document.querySelector('.custom-nav');
            const logo = document.querySelector('#logo');
            if (window.scrollY > 50) {
                navbar.classList.add('navbar-scroll');
                logo.classList.add('logo-small');
            } else {
                navbar.classList.remove('navbar-scroll');
                logo.classList.remove('logo-small');
            }
        }
    }
};
</script>
