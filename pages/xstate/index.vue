<template>
  <div class="container mx-auto px-24 my-16">
    <ContactForm />
  </div>
</template>

<script>
import NavRoutes from "~/components/NavRoutes/clients";
import ContactForm from "~/components/forms/contactForm";
export default {
  components: {
    NavRoutes,
    ContactForm
  }
};
</script>
