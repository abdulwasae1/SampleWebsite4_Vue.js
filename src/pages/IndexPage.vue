<template>
  <q-page class="gt-sm">
    <div class="q-mt-md">
      <q-img src="../assets/homepage-hero-background-3000-test.webp">
        <div
          style="background: none; margin-left: 4%; margin-top: 7%; width: 45%;"
        >
          <p class="text-deep-orange-7 text-weight-medium fontsize-30 no-margin">
            Sustainable Living
          </p>
          <p class="responsive-text2 no-margin">
            For Everyone
          </p>
          <p class="fontsize-10">
            Find vetted eco-friendly businesses in over 300 categories.
          </p>
          <div class="row">
            <div class="col-5 gt-md bg-white">
              <q-input
                borderless
                class="q-pa-xs"
                label="Search Product or Business"
              />
            </div>
            <div class="col-5 bg-white">
              <q-input
                v-model="text"
                borderless
                clearable
                class="q-pa-xs"
                placeholder="Your Location"
              />
            </div>
            <div class="col-lg-2 bg-white">
              <q-btn
                class=" q-ma-md"
                color="secondary"
                label="search"
              />
            </div>
          </div>
        </div>
      </q-img>
    </div>

    <div>
      <div class="q-pa-md">
        <div
          style="margin-left: 15%;"
          class="text-h4 text-green-9 text-weight-medium q-mb-lg"
        >
          CATEGORIES
        </div>
        <q-carousel
          v-model="slide"
          animated
          height="250px"
          navigation
          swipeable
          infinite
          control-color="grey"
          :autoplay="autoplay"
          transition-prev="slide-right"
          transition-next="slide-left"
          @mouseenter="autoplay = false"
          @mouseleave="autoplay = true"
        >
          <q-carousel-slide :name="1">
            <div class="row justify-between">
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/shirt-icon.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Clothing and Accessories
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-kids-1.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Kids
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-health&wellness.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Health & Wellness
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-outdoor.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Outdoors
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-reuse.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Reuse
                  </p>
                </div>
              </q-card>
            </div>
          </q-carousel-slide>
          <q-carousel-slide :name="2">
            <div class="row justify-between">
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-reuse.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Reuse
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-services.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Services
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/mobile-icon.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Tech
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-outdoor.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Outdoors
                  </p>
                </div>
              </q-card>
              <q-card class="col-2 cards q-pt-xl q-pb-md">
                <div class="row">
                  <div class="col-12 flex justify-center">
                    <q-img
                      src="../assets/icon-health&wellness.svg"
                      width="15%"
                    />
                  </div>
                  <p
                    class="col-12 flex justify-center q-mt-sm fontsize-8"
                    style="font-weight: 400;"
                  >
                    Health & Wellness
                  </p>
                </div>
              </q-card>
            </div>
          </q-carousel-slide>
        </q-carousel>
      </div>
    </div>

    <div class="flex justify-center text-h3">
      Better Businesses for Planet and People
    </div>

    <div class="q-mt-xl">
      <div
        class="q-gutter-md"
      >
        <q-img
          src="../assets/sustainability_simplified.svg"
          style="position: absolute;"
        />
        <div
          style=" margin-left: 15%; width: 80%;"
          class="q-mt-xl"
        >
          <h4
            class="text-green-9 text-weight-medium q-pt-xl"
            style="position: relative;"
          >
            SUSTAINABILITY<br>SIMPLIFIED
          </h4>
          <div class="row justify-evenly q-mt-xl">
            <div class="col-3 q-mt-xl">
              <q-card
                class="text-primary cards2"
              >
                <q-img
                  src="../assets/star.svg"
                  style="width: 45%; margin-left: 47%; position: absolute;"
                />

                <q-card-section>
                  <h5 class="text-orange-9 q-mb-lg text-weight-medium">
                    SHOP YOUR VALUES
                  </h5>
                  <p class="fontsize-8 text text-body1 no-margin no-padding">
                    Consumers who care about the environment, human rights, and making the world equitable
                    for all people need a place to find businesses aligned with these values. On iShopEco,
                    we identify many companies that use their revenue to make a positive impact.
                  </p>
                </q-card-section>
                <q-card-section>
                  <q-btn
                    :ripple="false"
                    flat
                    style="background: #dcf3e9; color: rgb(17, 15, 15); width: 100%;"
                    label="sustainability values"
                  />
                </q-card-section>
              </q-card>
            </div>
            <div class="col-3">
              <q-card
                class="text-primary cards2"
              >
                <q-img
                  src="../assets/world.svg"
                  style="width: 45%; margin-left: 47%; position: absolute;"
                />

                <q-card-section>
                  <h5 class="text-orange-9 q-mb-lg text-weight-medium">
                    SHOP EARTH-FRIENDLY
                  </h5>
                  <p class="fontsize-8 text text-weight-regular no-margin no-padding">
                    The businesses we feature meet essential environmental standards, including notable
                    eco-certifications, product transparency, fair trade operations, and more. The categories
                    used by businesses will help you easily find things that fit your lifestyle.
                  </p>
                </q-card-section>
                <q-card-section>
                  <q-btn
                    :ripple="false"
                    flat
                    style="background: #dcf3e9; color: rgb(17, 15, 15); width: 100%;"
                    label="sustainability guide"
                  />
                </q-card-section>
              </q-card>
            </div>
            <div class="col-3 q-mt-xl">
              <q-card
                class="text-primary cards2"
              >
                <q-img
                  src="../assets/home_location.svg"
                  style="width: 45%; margin-left: 47%; position: absolute;"
                />

                <q-card-section>
                  <h5 class="text-orange-9 q-mb-lg text-weight-medium">
                    SHOP LOCAL
                  </h5>
                  <p class="fontsize-8 text text-weight-regular no-margin no-padding">
                    Shopping at local businesses is the easiest way to reduce your environmental impact
                    and support job creation in your community. Browse companies in your area and share what you
                    find on social media to get friends involved!
                  </p>
                </q-card-section>
                <q-card-section>
                  <q-btn
                    :ripple="false"
                    flat
                    style="background: #dcf3e9; color: rgb(17, 15, 15); width: 100%;"
                    label="local benefits"
                  />
                </q-card-section>
              </q-card>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="row justify-center">
      <div class="col-3 q-mt-xl q-pt-md">
        <q-separator />
      </div>
      <div class="col-2">
        <div class="row justify-center q-pt-none">
          <h4 class="fontsize-14">
            You Are Helping
          </h4>
        </div>
      </div>
      <div class="col-3 q-mt-xl q-pt-md">
        <q-separator />
      </div>
    </div>

    <div class="row justify-center">
      <div class="col-7">
        <div
          style="text-align: center;"
          class="text-weight-regular fontsize-9"
        >
          There is an overwhelming amount of things to consider when building a green lifestyle. <br>
          By demanding brand transparency and buying responsibly-made products, you are taking the <br>
          first step in building a better world.
        </div>

        <div
          class="text-weight-medium fontsize-9 q-mt-lg"
          style="text-align: center;"
        >
          Shopping with retailers on iShopEco, you're taking action to:
        </div>
      </div>
    </div>

    <div class="q-mt-xl">
      <div class="row q-gutter-y-md">
        <div class="col-6">
          <q-card
            class="bg-blue-2"
            flat
            bordered
            style="width: 99%;"
          >
            <q-card-section horizontal>
              <q-img
                src="../assets/tick.svg"
                style="width: 15%; margin-left: 85%; position: absolute;"
              />
              <q-img
                class="col-7"
                src="../assets/istock-1.webp"
              />
              <q-card-section
                style="margin-top: 13%; text-align: center;"
                class="fontsize-10 text-weight-medium"
              >
                Increase job growth locally
              </q-card-section>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-6 flex justify-end">
          <q-card
            class="bg-deep-orange-5"
            flat
            bordered
            style="width: 99%;"
          >
            <q-card-section horizontal>
              <q-img
                src="../assets/tick.svg"
                style="width: 15%; margin-left: 27%; position: absolute;"
              />
              <q-card-section
                class="col-5 fontsize-10 text-weight-medium text-white"
                style="margin-top: 11%; text-align: center;"
              >
                Reduce your environmental footprint
              </q-card-section>

              <q-img
                class="col-7"
                src="../assets/istock-2.webp"
              />
            </q-card-section>
          </q-card>
        </div>
        <div class="col-6">
          <q-card
            class="bg-teal-4"
            flat
            bordered
            style="width: 99%;"
          >
            <q-card-section horizontal>
              <q-img
                src="../assets/tick.svg"
                style="width: 15%; margin-left: 85%; position: absolute;"
              />
              <q-img
                class="col-7"
                src="../assets/istock-3.webp"
              />
              <q-card-section
                class=" fontsize-9 text-weight-medium text-white"
                style="margin-top: 10%;"
              >
                Improve the social, economic, & environmental outlook for future generations
              </q-card-section>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-6 flex justify-end">
          <q-card
            class="bg-blue-2"
            flat
            bordered
            style="width: 99%;"
          >
            <q-card-section horizontal>
              <q-img
                src="../assets/tick.svg"
                style="width: 15%; margin-left: 27%; position: absolute;"
              />
              <q-card-section
                class="col-5 fontsize-10 text-weight-medium"
                style="margin-top: 10%; text-align: center;"
              >
                Inspire innovation in
                eco-friendly products & services
              </q-card-section>

              <q-img
                class="col-7"
                src="../assets/istock-4.webp"
              />
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>

    <div>
      <q-img
        src="../assets/bg-eco-grow-business-1920.svg"
        style="position: absolute;"
      />
      <div class="row justify-center">
        <div class="col-7">
          <q-card
            style="margin-top: 13%;"
            flat
            bordered
          >
            <q-card-section
              horizontal
              class="row"
            >
              <q-card-section class="col-6">
                <q-img
                  src="../assets/shoping-smily.svg"
                  style="width: 15%; margin-top: 8%;"
                />
                <p class="fontsize-12 text-weight-bold text-teal-7 no-margin">
                  Grow Your Business
                </p>
                <q-separator />
                <p class="fontsize-10 text-weight-medium text-teal-7 q-mt-sm">
                  Start by claiming your FREE listing!
                </p>
                <p class="fontsize-7 text-weigh-light">
                  Tailor your business page to reflect your company values and gain
                  visibility with eco-conscious local and national shoppers.
                </p>
                <q-btn
                  class="bg-orange-9 text-weight-medium text-white q-mt-lg"
                  style="width: 40%;"
                  flat
                >
                  learn more
                </q-btn>
              </q-card-section>

              <q-img
                src="../assets/bg-grow-business.webp"
              />
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>

    <div
      style="margin-top: 12%;"
    >
      <q-img src="../assets/group.png" />
    </div>

    <div
      class="row justify-center q-pb-xl gt-sm"
      style="background: #f36c21; margin-top: -1px;"
    >
      <div class="col-3 q-mt-xl">
        <div class="row">
          <div class="col-12 flex justify-center">
            <q-img
              src="../assets/ishopbusinesslogo.svg"
              style="width: 40%;"
            />
          </div>
        </div>
      </div>
      <div class="col-2 q-mt-xl">
        <p class="fontsize-8 text-weight-medium q-ml-md">
          ABOUT US
        </p>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label=" About us"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="careers"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="press"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="terms of service"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="sustainability"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="privacy policy"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="partners (TBD)"
        />
      </div>
      <div class="col-2 q-mt-xl">
        <p class="fontsize-8 text-weight-medium q-ml-md">
          FOR BUSINESSES
        </p>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="claim your business"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="advertising"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="sustainability guide"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="business support"
        />
      </div>
      <div class="col-2 q-mt-xl">
        <p class="fontsize-8 text-weight-medium q-ml-md">
          SUPPORT
        </p>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="get help"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="FAQs"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="contact us"
        />
        <br>
        <q-btn
          class="text-capitalize text-weight-regular text-subtitle1"
          flat
          style="color: #ffffff"
          label="business"
        />
      </div>
    </div>

    <div class="row justify-center bg-indigo-10 gt-sm">
      <div class="col-8">
        <div class="row justify-between">
          <div class="col-4 q-mt-xl q-mb-xl text-white">
            COPYRIGHT 2023. ISHOPECO. ALL RIGHTS RESERVED.
          </div>
          <div class="col-4 flex justify-end q-mt-xl q-mb-xl text-white">
            TERMS OF SERVICE | PRIVACY POLICY
          </div>
        </div>
      </div>
    </div>
  </q-page>
  <q-page
    class="lt-md"
    style=" background: #091f40;"
  >
    <div
      style="text-align: center;"
      class="bg-green-1"
    >
      <p class="fontsize-12 text-weight-light q-pa-md">
        iShopEco will go live 2023
      </p>
    </div>

    <div
      style="margin-top: -18px; width: inherit; background: #091f40;"
    >
      <div class="q-ml-sm">
        <p class="fontsize-26 no-margin q-pt-lg text-deep-orange-7 text-weight-medium">
          Sustainable Living
        </p>
        <p class="fontsize-18 no-margin text-white text-weight-normal">
          For Everyone
        </p>
        <p class="fontsize-14 text-white">
          Find Vetted Eco-Friendly Businesses in Over 300 Categories.
        </p>
      </div>
      <div class="row">
        <div class="col-8">
          <q-input
            class="bg-white q-ml-sm q-pl-sm q-pr-sm"
            placeholder="Search for business or product"
            style="border-radius: 7px;"
          />
          <q-input
            v-model="text"
            borderless
            clearable
            class="bg-white q-ml-sm q-mt-md q-pl-sm q-pr-sm"
            placeholder="Your Location"
            style="border-radius: 7px;"
          />
        </div>
      </div>
      <div style="height: 100%;">
        <div class="row justify-between">
          <div class="col-2">
            <q-btn
              class="bg-teal-6 text-white q-ml-sm q-mt-md"
              style="border-radius: 5px;"
            >
              search
            </q-btn>
          </div>
          <div class="col-sm-6 col-10 flex justify-end">
            <q-img
              src="../assets/hompage-hero-background-mobile.svg"
              style="width: 90%;"
            />
          </div>
        </div>
      </div>
    </div>
  </q-page>
</template>
/f36c21/
#091f40
<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  data () {
    return {
      selected: null,
      readonly: ref(false),
      disable: ref(false),
      text: ref('Huston, TX'),
      slide: ref(1),
      autoplay: ref(true)
    }
  }
})
</script>
