<script setup></script>

<template>
  <div class="pt-15 bg-grey-lighten-4 h-screen">
    <div class="d-flex flex-wrap ga-15 ms-15 mt-15">
      <v-card variant="grey" width="500px" class="ms-15">
        <v-card-text>
          <h1 class="text-h2 font-weight-black mt-15 text-blue">facebook</h1>
          <p class="mt-4 text-h5 font-weight-regular text-black">
            Facebook helps you connect and share with the people in your life.
          </p>
        </v-card-text>
      </v-card>
      <div class="ms-8">
        <v-card class="my-8" width="400" elevation="18">
          <v-card-item>
            <v-text-field
              v-model="email"
              :rules="emailRules"
              label="Email address or phone number"
              hide-details
              required
            ></v-text-field>
            <v-text-field
              class="mt-2"
              v-model="password"
              type="password"
              :rules="passwordRules"
              label="Password"
              hide-details
              required
            ></v-text-field>
            <v-btn type="submit" block class="mt-4 bg-blue tex-h6 mb-2"
              >Log in</v-btn
            >
            <a
              class="text-caption text-decoration-none text-blue ms-15 ps-15"
              href="#"
              rel="noopener noreferrer"
              target="_blank"
            >
              Forgot login password?</a
            >
            <v-divider class="mt-4"></v-divider>
            <v-btn color="green" class="mx-15 px-5 mt-6 mb-4" size="large">
              Create new account
            </v-btn>
          </v-card-item>
        </v-card>
        <p class="ms-8 text-body-2">
          <span class="font-weight-bold">Create a Page </span>for a celebrity,
          brand or business.
        </p>
      </div>
    </div>
  </div>
</template>
