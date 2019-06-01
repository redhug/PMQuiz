<template>
  <div id="app" 
      style="background-image: url('https://mdbootstrap.com/img/Photos/Others/architecture.jpg'); background-repeat: no-repeat; background-size: cover; background-position: center center;">

    <div class="row heading_style">
    <b-alert variant="success" show class="">Risk management questions</b-alert>
    </div>
    <HomePage answer="risk-averse" question="1) Risk utility rises at a decreasing rate for a _______ person."/>
    <HomePage answer="risk-seeking" question="2) Those who are ________ have a higher tolerance for risk, and their satisfaction increases when more payoff is at stake."/>
    <HomePage answer="risk-neutral" question="3) A ________ person achieves a balance between risk and payoff."/>
    <HomePage answer="Planning risk management" question="4) _________ involves deciding how to approach and plan the risk management activities for the project."/>
    <HomePage answer="Identifying risks" question="5) _________ involves prioritizing risks based on their probability and impact of occurrence."/>
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue'

export default {
  name: 'app',
  components: {
    HomePage
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  overflow-x: hidden;
}
.heading_style{
text-align:center;
font-size: 36px;
margin-left: 30% !important;
margin-top: 30px;
margin-bottom: 5%;
}
</style>
