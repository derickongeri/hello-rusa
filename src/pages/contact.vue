<template>
  <q-page class="flex flex-center">
    <div
      class="row items-center justify-center"
      style="width: 100vw; min-height: 15vh"
    >
      <div
        class="header-text text-h3 text-center q-my-lg"
        style="font-weight: 700"
      >
        Contact Us
      </div>
    </div>

    <div
      class="row items-center justify-center"
      style="width: 100vw;"
    >
      <div
        class="header-text header-caption text-h6 text-center "
        style="font-weight: 400"
      >
        We would love to hear from you
      </div>
    </div>
    <q-form
      @submit="submitForm"
      class="q-gutter-md q-pa-md"
      style="max-width: 600px; width: 100%"
    >
      <q-input
        v-model="name"
        label="Your Name"
        filled
        lazy-rules
        :rules="[(val) => !!val || 'Name is required']"
      />

      <q-input
        v-model="email"
        type="email"
        label="Your Email"
        filled
        lazy-rules
        :rules="[
          (val) => !!val || 'Email is required',
          (val) => /.+@.+\..+/.test(val) || 'Enter a valid email',
        ]"
      />

      <q-input
        v-model="message"
        label="Your Message"
        filled
        type="textarea"
        lazy-rules
        :rules="[(val) => !!val || 'Message is required']"
      />

      <div class="row tabs-desktop"><q-space/><q-btn unelevated no-caps label="Submit" type="submit" color="grey-10" style="border-radius: 10px;"/></div>

      <div class="row tabs-mobile"><q-btn unelevated no-caps label="Submit" type="submit" color="grey-10" style="border-radius: 10px;"/></div>

    </q-form>
  </q-page>
</template>

<script setup>
import { ref } from "vue";

const name = ref("");
const email = ref("");
const message = ref("");

const submitForm = async () => {
  if (!name.value || !email.value || !message.value) {
    console.error("Please fill out all fields");
    return;
  }

  const formData = {
    name: name.value,
    email: email.value,
    message: message.value,
  };

  try {
    const response = await fetch("https://your-api.com/contact", {
      method: "POST",
      headers: { "Content-Type": "application/json" },
      body: JSON.stringify(formData),
    });

    if (response.ok) {
      console.log("Message sent successfully");
      name.value = "";
      email.value = "";
      message.value = "";
    } else {
      console.error("Failed to send message");
    }
  } catch (error) {
    console.error("Error:", error);
  }
};
</script>
