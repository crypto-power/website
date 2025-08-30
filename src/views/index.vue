<script>
import {
    ArrowUpIcon ,
    MonitorIcon,
    FeatherIcon,
    EyeIcon,
    UserCheckIcon,
    SmartphoneIcon,
    HeartIcon,
    } from "vue-feather-icons";
import { Carousel, Slide } from "vue-carousel";
import countTo from "vue-count-to";

import Navbar from "@/components/navbar";
import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

export default {
  data() {
    return {};
  },
  components: {
    Navbar,
    Switcher,
    Footer,
    Carousel,
    Slide,
    ArrowUpIcon,
    countTo,
    Carousel,
    Slide,
    MonitorIcon,
    FeatherIcon,
    EyeIcon,
    UserCheckIcon,
    SmartphoneIcon,
    HeartIcon,
  },
};
</script>

<template>
  <div>
    <Navbar />
    <!-- Hero Start -->
    <section
      class="bg-half-170 d-table w-100 overflow-hidden"
      id="home"
    >
      <div class="container">
        <div class="row mt-5 align-items-center">
          <div class="col-lg-6 col-md-7">
            <div class="title-heading">
              <h1 class="heading mb-3">
                Stay in control of your assets with
                <span class="text-primary">Cryptopower</span> wallet
              </h1>
              <p class="para-desc text-muted">
                multi-coin wallet for DCR, BTC, and LTC with integrated DCRDEX support, available on desktop and mobile.
              </p>
              <div class="mt-4">
                <a
                  href="https://apps.apple.com/us/app/cryptopower-wallet/id6472668308"
                  target="_blank"
                  class="btn btn-outline-primary mt-2 mr-2"
                ><i class="mdi mdi-apple"></i> App Store</a>
                <a
                  href="https://play.google.com/store/apps/details?id=com.dreacotdigital.cryptopower.mainnet"
                  target="_blank"
                  class="btn btn-outline-primary mt-2"
                ><i class="mdi mdi-google-play"></i> Play Store</a>
              </div>
                <div class="mt-4">
        <div
          class="buy-button"
          v-if="isIcons !== true"
        >
          <a
            href=""
            target="_blank"
            class="btn"
            v-scroll-to="'#downloads'"
            :class="{
              'btn-light': navLight === true,
              'btn-primary': navLight !== true,
            }"
          >Download for Desktop</a>
          </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-6 col-md-5 mt-4 pt-2 mt-sm-0 pt-sm-0">
            <div class="text-md-right text-center ml-lg-4">
              <img
                src="images/app/iphone.png"
                height=600
                class=" mover mx-auto d-block "
                alt=""
              >
            </div>
          </div>
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Hero End -->

    <!-- TABLE START -->
    <section class="section border-top">
      <!-- Table Start -->
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-12 col-lg-10">
            <div class="table-responsive features-absolute bg-white shadow-md rounded-md">
              <table class="table mb-0 table-center">
                <thead>
                  <tr>
                    <th scope="col">#</th>
                    <th
                      scope="col"
                      style="min-width: 250px;"
                    >Name</th>
                    <th
                      scope="col"
                      style="width: 150px;"
                    >Price</th>
                    <th
                      scope="col"
                      style="width: 100px;"
                    >Change</th>
                    <!-- <th
                      scope="col"
                      style="width: 100px;"
                    >Trade</th> -->
                  </tr>
                </thead>
                <tbody>

                  <tr>
                    <td scope="row">1</td>
                    <th>
                      <div class="d-flex align-items-center">
                        <img
                          src="images/crypto/logo_dcr_blue.png"
                          class="float-left mr-3"
                          height="50"
                          alt=""
                        >
                        <p class="mb-0 font-weight-normal h5">Decred <span class="text-muted h6">DCR</span> </p>
                      </div>
                    </th>
                    <td>$17.68</td>
                    <td class="text-danger">-1.9</td>
                    <!-- <td><a
                        href="javascript:void(0)"
                        class="btn btn-primary"
                      >Buy</a></td> -->
                  </tr>

                  <tr>
                    <td scope="row">2</td>
                    <th>
                      <div class="d-flex align-items-center">
                        <img
                          src="images/crypto/logo_btc.png"
                          class="float-left mr-3"
                          height="50"
                          alt=""
                        >
                        <p class="mb-0 font-weight-normal h5">Bitcoin <span class="text-muted h6">BTC</span> </p>
                      </div>
                    </th>
                    <td>$ 113,000.68</td>
                    <td class="text-danger">-2.5</td>
                    <!-- <td><a
                        href="javascript:void(0)"
                        class="btn btn-primary"
                      >Buy</a></td> -->
                  </tr>

                  <tr>
                    <td scope="row">3</td>
                    <th>
                      <div class="d-flex align-items-center">
                        <img
                          src="images/crypto/logo_ltc.png"
                          class="float-left mr-3"
                          height="50"
                          alt=""
                        >
                        <p class="mb-0 font-weight-normal h5">Litecoin <span class="text-muted h6">LTC</span></p>
                      </div>
                    </th>
                    <td>$ 134.43</td>
                    <td class="text-success">+.264</td>
                    <!-- <td><a
                        href="javascript:void(0)"
                        class="btn btn-primary"
                      >Buy</a></td> -->
                  </tr>
                </tbody>
              </table>
              <!--end table-->
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <!-- Table End -->
    </section>

    <!-- About start -->
    <section id="about" class="section">
      <!-- Crypto Portfolio end -->
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-12 text-center">
            <div class="section-title mb-4 pb-2">
              <h4 class="title mb-4">A cross-platform SPV (DCR, BTC & LTC) privacy wallet built with go.</h4>
              <p class="text-muted para-desc mb-0 mx-auto">Cryptopower is a self-custodial multi-coin wallet built by an open-source community of developers from around the world.
                The app is built using Gio, a Golang library that facilitates the implementation of cross-platform immediate mode user interfaces.
              </p>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->

        <div class="row">
          <div class="col-12 mt-4 pt-2">
            <img
              src="images/app/ipad01.png"
              class="img-fluid mx-auto d-block"
              alt=""
            >
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <!-- Crypto Portfolio end -->
    <!--end section-->
    <!-- Testi n Download cta End -->
    </section>

    <!-- Features Start -->
    <section id="features" class="section bg-light">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-12 text-center">
            <div class="section-title mb-4 pb-2">
              <h4 class="title mb-4">App Features</h4>
              <p class="text-muted para-desc mb-0 mx-auto">
                <span class="text-primary font-weight-bold">Cryptopower</span> offers a robust suite of features built for security, 
                privacy, and user control.
              </p>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->

        <div class="row justify-content-center align-items-center">
          <div class="col-lg-8 col-md-8">
            <div class="row mt-4 pt-2">
              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <monitor-icon
                      class="fea icon-ex-md text-primary"
                    ></monitor-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Self-Custodial Control</h4>
                    <p class="text-muted para mb-0">
                      You hold your keys, you control your funds. True self-sovereignty.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <feather-icon
                      class="fea icon-ex-md text-primary"
                    ></feather-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Enhanced Privacy</h4>
                    <p class="text-muted para mb-0">
                      Built-in decentralized coin mixing for Decred transactions.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <eye-icon class="fea icon-ex-md text-primary"></eye-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Multi-Coin Support</h4>
                    <p class="text-muted para mb-0">
                        Manage DCR, BTC & LTC wallets.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <user-check-icon
                      class="fea icon-ex-md text-primary"
                    ></user-check-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Integrated DCR Staking</h4>
                    <p class="text-muted para mb-0">
                      Stake Decred directly to earn rewards and participate in governance.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <smartphone-icon
                      class="fea icon-ex-md text-primary"
                    ></smartphone-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Trustless P2P Trading</h4>
                    <p class="text-muted para mb-0">
                      Trade directly peer-to-peer via atomic swaps on DCRDEX. No intermediaries, no custodial risk.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <heart-icon
                      class="fea icon-ex-md text-primary"
                    ></heart-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Lightweight & Fast</h4>
                    <p class="text-muted para mb-0">
                        Uses SPV wallets for quick sync without full blockchain downloads.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

                <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <smartphone-icon
                      class="fea icon-ex-md text-primary"
                    ></smartphone-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Multi seed support</h4>
                    <p class="text-muted para mb-0">
                      Import 12, 24 & 33-word seed from other wallets.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-md-6 col-12">
                <div class="media features pt-4 pb-4">
                  <div
                    class="icon text-center rounded-circle text-primary mr-3 mt-2"
                  >
                    <heart-icon
                      class="fea icon-ex-md text-primary"
                    ></heart-icon>
                  </div>
                  <div class="media-body">
                    <h4 class="title">Coin Control</h4>
                    <p class="text-muted para mb-0">
                       Select exact outputs to be used in the transaction, take full control of your privacy.
                    </p>
                  </div>
                </div>
              </div>
              <!--end col-->
            </div>
            <!--end row-->
          </div>
          <!--end col-->

          <div
            class="col-lg-4 col-md-4 col-12 mt-4 pt-2 text-center text-md-right"
          >
            <img src="images/app/iphone_2.png" class="img-fluid" alt="" />
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Feature End -->

     <!-- Download cta start -->
    <section id="downloads" class="section">
      <div class="container">

        <div
          class="row mt-md-5 pt-md-3 mt-4 pt-2 mt-sm-0 pt-sm-0 justify-content-center"
        >
          <div class="col-12 text-center">
            <div class="section-title">
              <h4 class="title mb-4">Download Cryptopower Wallet</h4>
              <p class="text-muted para-desc mx-auto">
                Choose the right version for your operating system and install Cryptopower Wallet to securely manage, send, and exchange your crypto with ease anytime, anywhere.
              </p>
              <div class="mt-4">
                <a class="" href="https://github.com/crypto-power/cryptopower/releases"
                    target="_blank">Mac OS ↓ <span style="margin-left: 5px;">| </span></a>
                <a class=""
                    href="https://github.com/crypto-power/cryptopower/releases"
                    target="_blank">Linux ↓ <span style="margin-left: 5px;">| </span></a>
                <a class="add-margin"
                    href="https://github.com/crypto-power/cryptopower/releases"
                    target="_blank">Windows ↓ <span style="margin-left: 5px;">| </span></a>
                <a class="add-margin"
                    href="https://github.com/crypto-power/cryptopower/releases"
                    target="_blank">FreeBSD ↓ <span style="margin-left: 5px;">| </span></a>
                    <a class="add-margin"
                    href="https://github.com/crypto-power/cryptopower/releases"
                    target="_blank">Android (APK) ↓ <span style="margin-left: 5px;">| </span></a>
                <a class="add-margin" href="https://github.com/crypto-power/cryptopower/releases" target="_blank">Release Notes
                    →</a>
              </div>

              <div class="mt-4">
                <a 
                  href="https://apps.apple.com/us/app/cryptopower-wallet/id6472668308"
                  target="_blank"
                  class="btn btn-primary mt-2 mr-2"
                  ><i class="mdi mdi-apple"></i> App Store</a
                >
                <a
                  href="https://play.google.com/store/apps/details?id=com.dreacotdigital.cryptopower.mainnet"
                  target="_blank"
                  class="btn btn-primary mt-2"
                  ><i class="mdi mdi-google-play"></i> Play Store</a
                >
              </div>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Section End -->

    <section id="faq" class="section">
      <!-- Rate Start -->
      <div class="container mt-100 mt-60">
        <div class="row align-items-center">
          <div class="col-lg-12 col-md-12 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <div class="ml-lg-4">
              <div class="section-title mb-4 pb-2 text-center">
                <h4 class="title mb-4">Frequently asked questions</h4>
                <p class="text-muted para-desc mb-0 mx-auto">Find answers to common questions</p>
              </div>

              <div class="faq-content mt-4">
                <div
                  class="accordion"
                  id="accordionExampleone"
                >
                  <b-card
                    no-body
                    class="mb-2 border-0 rounded"
                  >
                    <b-card-header class="border-0 bg-light p-3 pr-5">
                      <a
                        class="faq position-relative text-dark"
                        v-b-toggle.accordion-1
                        href="javascript: void(0);"
                      >
                        <h6 class="title mb-0"> What is Cryptopower Wallet? </h6>
                      </a>
                    </b-card-header>
                    <b-collapse
                      id="accordion-1"
                      visible
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body class="px-2 py-4">
                        <p class="text-muted mb-0 faq-ans">Cryptopower is a self-custodial Decred wallet application designed for both desktop and mobile platforms. 
                            It offers support for creating wallets not only for Decred but also for other cryptocurrencies such as Bitcoin and Litecoin. 
                            <br><br> The app is built using Gio, a Golang library that facilitates the implementation of cross-platform immediate mode user interfaces. 
                            By leveraging a tightly integrated Golang codebase, Cryptopower delivers a native app experience that is smaller, faster, and more efficient for the Decred ecosystem.

</p>
                      </b-card-body>
                    </b-collapse>
                  </b-card>
                  <b-card
                    no-body
                    class="mb-2 border-0 rounded"
                  >
                    <b-card-header class="border-0 bg-light p-3 pr-5">
                      <a
                        class="faq position-relative text-dark"
                        v-b-toggle.accordion-2
                        href="javascript: void(0);"
                      >
                        <h6 class="title mb-0"> Does Crytopower support my favorite crypto?</h6>
                      </a>
                    </b-card-header>
                    <b-collapse
                      id="accordion-2"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body class="px-2 py-4">
                        <p class="text-muted mb-0 faq-ans">We’re proud to support some of the most popular cryptocurrencies available today:

                            <br><br>- Decred (DCR)
                            <br>- Bitcoin (BTC)
                            <br>- Litecoin (LTC)<br><br>

                            Is there a coin you’d like to see added? Let us know on our socials or join the conversation via the community, we’d love to hear from you!
                        </p>
                      </b-card-body>
                    </b-collapse>
                  </b-card>
                  <b-card
                    no-body
                    class="mb-2 border-0 rounded"
                  >
                    <b-card-header class="border-0 bg-light p-3 pr-5">
                      <a
                        class="faq position-relative text-dark"
                        v-b-toggle.accordion-3
                        href="javascript: void(0);"
                      >
                        <h6 class="title mb-0"> I need help, where can I reach out?</h6>
                      </a>
                    </b-card-header>
                    <b-collapse
                      id="accordion-3"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body class="px-2 py-4">
                        <p class="text-muted mb-0 faq-ans">Our support team is here for you 24/7. You can reach us anytime through the app (just tap “Help” in the Settings), on our website (click                 <router-link to="" v-scroll-to="'#support'" class="text-foot"
                  >
                  Support</router-link
                >), or via email <a href="mailto:support@cryptopower.dev" class="text-primary mt-3 mb-0">support@cryptopower.dev</a>.

                            <br><br> We are always happy to point you in the right direction!</p>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card
                    no-body
                    class="mb-2 border-0 rounded"
                  >
                    <b-card-header class="border-0 bg-light p-3 pr-5">
                      <a
                        class="faq position-relative text-dark"
                        v-b-toggle.accordion-4
                        href="javascript: void(0);"
                      >
                        <h6 class="title mb-0"> Is Cryptopower open-source? </h6>
                      </a>
                    </b-card-header>
                    <b-collapse
                      id="accordion-4"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body class="px-2 py-4">
                        <p class="text-muted mb-0 faq-ans">The Cryptopower project is an open-source initiative, see us on <a
              href="https://github.com/crypto-power/cryptopower"
              target="_blank"
              class=""
            >Github</a></p>
                      </b-card-body>
                    </b-collapse>
                  </b-card>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <!-- Rate End -->
    </section>

    <!-- Start Section -->
    <section id="support" class="section">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-12">
                    <div class="section-title text-center mb-4 pb-2">
                        <h4 class="mb-4">Find the help you need</h4>
                        <p class="para-desc mx-auto text-muted">Get help with Cryptopower Wallet by reaching out to the active Decred community</p>
                    </div>
                </div>
                <!--end col-->
            </div>
            <!--end row-->

            <div class="row justify-content-center">
                <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                    <div class="card explore-feature border-0 rounded text-center bg-white">
                        <div class="card-body">
                            <div class="icon rounded-circle shadow-lg d-inline-block mb-2 h2">
                                <i class="uil uil-chat"></i>
                            </div>
                            <div class="content mt-3">
                                <router-link to="" href="https://matrix.to/#/#cryptopower:decred.org" target="_blank" class="title h5 text-dark">Matrix</router-link>
                                <p class="text-muted mt-3 mb-0">Community Support</p>
                            </div>
                        </div>
                    </div>
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                    <div class="card explore-feature border-0 rounded text-center bg-white">
                        <div class="card-body">
                            <div class="icon rounded-circle shadow-lg d-inline-block mb-2 h2">
                                <i class="uil uil-twitter"></i>
                            </div>
                            <div class="content mt-3">
                                <router-link to="" href="https://twitter.com/cryptopowerwlt" target="_blank" class="title h5 text-dark">Twitter</router-link>
                                <p class="text-muted mt-3 mb-0">Community Support</p>
                            </div>
                        </div>
                    </div>
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                    <div class="card explore-feature border-0 rounded text-center bg-white">
                        <div class="card-body">
                            <div class="icon rounded-circle shadow-lg d-inline-block mb-2 h2">
                                <i class="uil uil-telegram-alt"></i>
                            </div>
                            <div class="content mt-3">
                                <router-link to="" href="https://t.me/cryptopowerwallet" target="_blank" class="title h5 text-dark">Telegram</router-link>
                                <p class="text-muted mt-3 mb-0">Community Support</p>
                            </div>
                        </div>
                    </div>
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                    <div class="card explore-feature border-0 rounded text-center bg-white">
                        <div class="card-body">
                            <div class="icon rounded-circle shadow-lg d-inline-block mb-2 h2">
                                <i class="uil uil-envelope-alt"></i>
                            </div>
                            <div class="content mt-3">
                                <a to href="mailto:support@cryptopower.dev" class="title h5 text-dark">Email</a>
                                <p class="text-muted mt-3 mb-0"><a href="mailto:support@cryptopower.dev" class="text-primary mt-3 mb-0">support@cryptopower.dev</a></p>
                            </div>
                        </div>
                    </div>
                </div>
                <!--end col-->
            </div>
            <!--end row-->
        </div>
        <!--end container-->
    </section>
    <!--end section-->
    <!-- Section END -->

    <!--end section-->
    <Footer />
    <!-- Footer End -->
    <Switcher />
    <!-- Back to top -->
    <a
      href="javascript: void(0);"
      class="btn btn-icon btn-primary back-to-top"
      id="back-to-top"
      v-scroll-to="'#topnav'"
    >
      <arrow-up-icon class="icons"></arrow-up-icon>
    </a>
    <!-- Back to top -->
  </div>
</template>
