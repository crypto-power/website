<script>
import Switcher from "@/components/switcher";
import {
    HomeIcon
} from 'vue-feather-icons';

/**
 * Page-error component
 */
export default {
    data() {
        return {}
    },
    components: {
        Switcher,
        HomeIcon
    }
}
</script>

<template>
<div>
    <div class="back-to-home rounded d-none d-sm-block">
        <router-link to="/" class="btn btn-icon btn-soft-primary">
            <home-icon class="icons"></home-icon>
        </router-link>
    </div>

    <!-- ERROR PAGE -->
    <section class="bg-home d-flex align-items-center">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8 col-md-12 text-center">
                <div>
                <router-link
                    class="logo"
                    to="/"
                    v-scroll-to="'#home'"
                    v-if="navLight !== true"
                >
                    <img
                    src="images/logo-dark.png"
                    height="60"
                    alt=""
                    />
                </router-link>
                <router-link
                    class="logo"
                    to="/"
                    v-scroll-to="'#home'"
                    v-else
                >
                    <img
                    src="images/logo-dark.png"
                    class="l-dark"
                    height="60"
                    alt=""
                    />
                    <img
                    src="images/logo-light.png"
                    class="l-light"
                    height="60"
                    alt=""
                    />
                </router-link>
                </div>
                    <img src="images/404.svg" class="img-fluid" alt="">
                    <div class="text-uppercase mt-4 display-3">Oh ! no</div>
                    <div class="text-capitalize text-dark mb-4 error-page">Page Not Found</div>
                </div>
                <!--end col-->
            </div>
            <!--end row-->

            <div class="row">
                <div class="col-md-12 text-center">
                    <router-link to="/" class="btn btn-outline-primary mt-4">Go Back</router-link>
                    <router-link to="/" class="btn btn-primary mt-4 ml-2">Go To Home</router-link>
                </div>
                <!--end col-->
            </div>
            <!--end row-->
        </div>
        <!--end container-->
    </section>
    <!--end section-->
    <!-- ERROR PAGE -->
    <Switcher />
</div>
</template>
