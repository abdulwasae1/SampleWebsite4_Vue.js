<template>
  <q-layout class="gt-sm">
    <q-header
      class="firstheading"
    >
      <div>
        <q-img
          src="~assets/consumer-header.svg"
          alt=""
          style="position: absolute;"
        />
        <q-toolbar>
          <q-toolbar-title class="flex justify-center q-mt-md gt-md">
            <p class="fontsize-9">
              iShopEco will go live 2023
            </p>
          </q-toolbar-title>
        </q-toolbar>
        <div class="row shadow-4 q-pb-md">
          <div class="col-2">
            <q-img
              src="~assets/consumer-logo-desktop.png"
              style="width: 127px;"
              class="q-mt-xl q-ml-lg"
            />
          </div>
          <div class="col-10">
            <div class="row q-mt-md">
              <div class="col-6 flex justify-end">
                <q-btn
                  flat
                  class="text-subtitle1
                  text-weight-bold"
                  color="grey-13"
                  icon-right="search"
                  label="search"
                />
                <q-input
                  v-model="text"
                  clearable
                  dense
                  class="q-ml-xl q-mt-md"
                  color="grey-13"
                  placeholder="Your Location"
                  icon="edit"
                />
              </div>
              <div class="col-3 flex justify-center">
                <div class="q-pa-md">
                  <q-btn-dropdown
                    flat
                    class="
                    bg-white
                    text-weight-regular
                    text-capitalize
                    text-body1"
                    label="Eco Brands"
                  >
                    <q-list>
                      <q-item
                        v-close-popup
                        clickable
                        @click="onItemClick"
                      >
                        <q-item-section>
                          <q-item-label>Photos</q-item-label>
                        </q-item-section>
                      </q-item>

                      <q-item
                        v-close-popup
                        clickable
                        @click="onItemClick"
                      >
                        <q-item-section>
                          <q-item-label>Videos</q-item-label>
                        </q-item-section>
                      </q-item>

                      <q-item
                        v-close-popup
                        clickable
                        @click="onItemClick"
                      >
                        <q-item-section>
                          <q-item-label>Articles</q-item-label>
                        </q-item-section>
                      </q-item>
                    </q-list>
                  </q-btn-dropdown>
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col-12 q-mt-md">
                <div class="row">
                  <div class="col-xl-1" />
                  <div class=" col-xl-9 gt-md">
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Clothing & Accessories
                    </q-btn>
                    <span><b
                      style="color: rgb(7, 141, 14);"
                    >l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      kids
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Health & Wellness
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Home Goods
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Outdoors
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      pets
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Reuse
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Services
                    </q-btn>
                    <span><b style="color: rgb(7, 141, 14);">l</b></span>
                    <q-btn
                      flat
                      class="text-capitalize text-subtitle1"
                    >
                      Tech
                    </q-btn>
                  </div>
                  <div class="col flex justify-end">
                    <q-btn
                      color="brand"
                      icon="business"
                      label="For Business"
                      class="text-capitalize text-subtitle1 gt-md"
                    />
                    <q-btn
                      flat
                      color="dark"
                      icon="menu"
                    >
                      <q-menu>
                        <q-list style="min-width: 100px">
                          <q-item
                            v-close-popup
                            clickable
                          >
                            <q-item-section>New tab</q-item-section>
                          </q-item>
                          <q-item
                            v-close-popup
                            clickable
                          >
                            <q-item-section>New incognito tab</q-item-section>
                          </q-item>
                          <q-separator />
                          <q-item
                            v-close-popup
                            clickable
                          >
                            <q-item-section>Recent tabs</q-item-section>
                          </q-item>
                        </q-list>
                      </q-menu>
                    </q-btn>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>

  <q-layout
    view="lhr lpr fFf"
    class="lt-md"
  >
    <q-header
      reveal
      class="bg-white text-dark q-pt-sm"
    >
      <q-toolbar>
        <q-toolbar-title>
          <img
            style="margin-left: 49.5%;"
            src="../assets/consumer-logo-mobile.png"
          >
        </q-toolbar-title>

        <q-btn
          dense
          flat
          round
          icon="menu"
          @click="toggleRightDrawer"
        />
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="rightDrawerOpen"
      side="right"
      overlay
      elevated
    >
      <q-btn
        borderless
        flat
      >
        hello
      </q-btn>
      <!-- drawer content -->
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer
      reveal
      class="bg-white text-dark"
    >
      <div class="row justify-evenly">
        <div class="col-2 flex justify-center">
          <q-btn
            flat
            borderless
            class="text-capitalize text-weight-regular fontsize-9"
          >
            <q-img
              src="../assets/search_icon.svg"
              style="width: 55%;"
            />
            search
          </q-btn>
        </div>
        <div class="col-2 flex justify-center">
          <q-btn
            flat
            borderless
            class="text-capitalize text-weight-regular fontsize-9"
          >
            <q-img
              src="../assets/category.svg"
              style="width: 45%;"
            />
            categories
          </q-btn>
        </div>
        <div class="col-2 flex justify-center">
          <q-btn
            flat
            borderless
            class="text-capitalize text-weight-regular fontsize-9"
          >
            <q-img
              src="../assets/eco.svg"
              style="width: 60%;"
            />
            brands
          </q-btn>
        </div>
        <div class="col-2 flex justify-center">
          <q-btn
            flat
            borderless
            class="text-capitalize text-weight-regular fontsize-9"
          >
            <q-img
              src="../assets/info.svg"
              style="width: 100%;"
            />
            info
          </q-btn>
        </div>
        <div class="col-2 flex justify-center">
          <q-btn
            flat
            borderless
            class="text-capitalize text-weight-regular fontsize-9"
          >
            <q-img
              src="../assets/feed.svg"
              style="width: 65%;"
            />
            news
          </q-btn>
        </div>
      </div>
    </q-footer>
  </q-layout>
</template>
<script>
import { ref } from 'vue'

export default {
  setup () {
    const rightDrawerOpen = ref(false)
    return {
      text: ref('Huston, TX'),
      rightDrawerOpen,
      toggleRightDrawer () {
        rightDrawerOpen.value = !rightDrawerOpen.value
      }
    }
  }
}

</script>
<style>
.firstheading {
  color: rgb(44, 44, 44);
  background: none;
}
.bg-brand {
  background: #862b01 !important;
}
</style>
