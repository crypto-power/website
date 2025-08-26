<script>
import {
  FacebookIcon,
  InstagramIcon,
  TwitterIcon,
  LinkedinIcon,
  MailIcon,
} from "vue-feather-icons";
export default {
  data() {
    return {};
  },
  components: {
    FacebookIcon,
    InstagramIcon,
    TwitterIcon,
    LinkedinIcon,
    MailIcon,
  },
};
</script>

<template>
  <div>
    <!-- Footer Start -->
    <footer class="footer">
      <div class="container">
        <div class="row">
          <div class="col-lg-4 col-12 mb-0 mb-md-4 pb-0 pb-md-2">
            <a href="" v-scroll-to="'#home'" class="logo-footer">
              <img src="images/logo-light.png" height="48" alt="" />
            </a>
            <p class="mt-4">
              multi-coin wallet for DCR, BTC, and LTC with integrated DCRDEX support, available on desktop and mobile.
            </p>
            <ul class="list-unstyled social-icon social mb-0 mt-4">
              <li class="list-inline-item ml-1">
                <a href="https://x.com/cryptopowerWlt" target="_blank" class="rounded">
                  <twitter-icon class="fea icon-sm fea-social"></twitter-icon>
                </a>
              </li>
            </ul>
            <!--end icon-->
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-4 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <h5 class="text-light footer-head">Company</h5>
            <ul class="list-unstyled footer-list mt-4">
              <li>
                <router-link to="" v-scroll-to="'#about'" class="text-foot"
                  > About </router-link
                >
              </li>
              <li>
                <router-link to="" v-scroll-to="'#features'" class="text-foot"
                  >
                  Features</router-link
                >
              </li>
              <li>
                <router-link to="" v-scroll-to="'#downloads'" class="text-foot"
                  > Downloads</router-link
                >
              </li>
              <li>
                <router-link to="" v-scroll-to="'#faq'" class="text-foot"
                  >
                  FAQ</router-link
                >
              </li>
              <li>
                <router-link to="" v-scroll-to="'#support'" class="text-foot"
                  >
                  Support</router-link
                >
              </li>
            </ul>
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-4 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <h5 class="text-light footer-head">Useful Links</h5>
            <ul class="list-unstyled footer-list mt-4">
              <li>
                <router-link to="" class="text-foot"
                  > Terms of
                  Services</router-link
                >
              </li>
              <li>
                <router-link to="" class="text-foot"
                  > Privacy
                  Policy</router-link
                >
              </li>
              <li>
                <router-link to="" href="https://docs.decred.org/" target="_blank" class="text-foot"
                  >
                  Documentation</router-link
                >
              </li>
            </ul>
          </div>
          <!--end col-->

        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </footer>
    <!--end footer-->
    <footer class="footer footer-bar">
      <div class="container text-center">
        <div class="row align-items-center">
          <div class="col-sm-6">
            <div class="text-sm-left">
              <p class="mb-0">
                © {{ new Date().getFullYear() }} Cryptopower Developers.
              </p>
            </div>
          </div>
          <!--end col-->

        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </footer>
    <!--end footer-->
  </div>
</template>
