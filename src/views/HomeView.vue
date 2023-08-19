<template>
  <div class="home">
    <!-- <Feature/> -->
    <!-- <About/> -->
  <!-- <ReportAbuse/> -->
    <!-- <Privacy/> -->
    <!-- <RegisterLogin/> -->
    <ResetPassword/>
    <Footer /> 
  </div>
</template>

<script>
import About from "./About.vue";
import Feature from "../views/Features.vue"
import Footer from "../components/Footer.vue"
import Privacy from "./Privacy.vue"
import ReportAbuse from "./ReportAbuse.vue";
import RegisterLogin from "@/components/RegisterLogin.vue";
import ResetPassword from "./ResetPassword.vue";
export default {
  name: 'HomeView',
  components: {
    Feature,
    About,
    Privacy,
    Footer,
    ReportAbuse,
    RegisterLogin,
    ResetPassword
}
}
</script>
