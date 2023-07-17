<script>
import ContactForm from './components/Contact.vue'
import About from './components/About.vue'
import Header from './components/Header.vue'
import Team from './components/OurTeam.vue'
import Price from './components/Price.vue'
import UserInfo from './components/UserInfo.vue'

export default {
  components: {
    Header,
    About,
    Price,
    Team,
    UserInfo,
    ContactForm,

  },
}
</script>

<template>
  <Header></Header>
  <About></About>
  <Price></Price>
  <Team></Team>
  <UserInfo></UserInfo>
  <ContactForm></ContactForm>
</template>

<style></style>
