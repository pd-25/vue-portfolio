<template>
  <v-container class="my-5">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center"> Contact Me</v-subheader>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, rerum.</p>
      </v-col>
      <v-col lg="6" class="mt-10">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d29472.587482245315!2d88.41647338042657!3d22.576356601559088!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a0275b020703c0d%3A0xece6f8e0fc2e1613!2sSector%20V%2C%20Bidhannagar%2C%20Kolkata%2C%20West%20Bengal!5e0!3m2!1sen!2sin!4v1683698601029!5m2!1sen!2sin"
          width="100%"
          height="100%"
          style="border: 0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </v-col>

      <v-col lg="6" class="mt-10">
        <form>
          <v-text-field
            v-model="contactInfo.name"
            :counter="10"
            label="Name"
          ></v-text-field>

          <v-text-field
            v-model="contactInfo.phone"
            :counter="7"
            label="Phone Number"
          ></v-text-field>

          <v-text-field v-model="contactInfo.email" label="E-mail"></v-text-field>

          <v-btn class="me-4" color="success" type="submit"> submit </v-btn>
        </form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      contactInfo: {},
    };
  },
};
</script>
