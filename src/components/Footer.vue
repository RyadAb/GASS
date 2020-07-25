<template>
  <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="deep-purple accent-4 white--text text-center"
      style="width:100%"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-text>

      <div class=" text-center text-md-left">

    <!-- Grid row -->
    <div class="row">

      <!-- Grid column -->
      <div class="col-md-4 mx-auto">

        <!-- Content -->
        <p class="h5 font-italic mt-9 mb-6">"Reason, observation, and experience; the holy trinity of science."</p>
        <p class="">Robert Green Ingersoll</p>
      </div>
      <!-- Grid column -->

      <hr class="clearfix w-100 d-md-none">

      <!-- Grid column -->
      <div class="col-md-2 mx-auto">

        <!-- Links -->
        <h5 class="font-weight-bold text-uppercase mt-3 mb-4">GASS</h5>

        <ul class="list-unstyled">
          <li>
            <a href="#!" style="color:white">History</a>
          </li>
          <li>
            <a href="#!" style="color:white">Mission and Objectives</a>
          </li>
          <li>
            <a href="#!" style="color:white">Status</a>
          </li>
          <li>
            <a href="#!" style="color:white">Rules</a>
          </li>
          <li>
            <a href="#!" style="color:white">Members</a>
            <ul class="list-unstyled">
              <li>
                <a href="#!" style="color:white">Founders members</a>
              </li> 
              <li>
                <a href="#!" style="color:white">Associate members</a>
              </li> 
            </ul>
          </li>
        </ul>

      </div>
      <!-- Grid column -->

      <hr class="clearfix w-100 d-md-none">

      <!-- Grid column -->
      <div class="col-md-2 mx-auto">

        <!-- Links -->
        <h5 class="font-weight-bold text-uppercase mt-3 mb-4">ACTIVITIES</h5>

        <ul class="list-unstyled">
          <li>
            <a href="#!" style="color: white">Link 1</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 2</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 3</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 4</a>
          </li>  
        </ul>

      </div>
      <!-- Grid column -->

      <hr class="clearfix w-100 d-md-none">

      <!-- Grid column -->
      <div class="col-md-2 mx-auto">

        <!-- Links -->
        <h5 class="font-weight-bold text-uppercase mt-3 mb-4">PUBLICATIONS</h5>

        <ul class="list-unstyled">
          <li>
            <a href="#!" style="color: white">Link 1</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 2</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 3</a>
          </li>
          <li>
            <a href="#!" style="color: white">Link 4</a>
          </li>
        </ul>

      </div>
      <!-- Grid column -->

    </div>
    <!-- Grid row -->

  </div>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>GASS</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>