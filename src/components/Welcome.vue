<template>
    <div class="Welcome-Intranse">
        <h1>{{ msg }}</h1>
        <p>This is My Final Project in Web System and Technologies using VueJs and Vue CLI tools</p>
        <br><br>
        <!-- Footer --> 
            <div id="footer"> 
            <div class="footer container"> 
                <div class="brand"> 
                <h1><span>E</span>lements <span>P</span>ortfolio</h1> 
                </div> 
                <h2>My Complete Web Portfolio</h2> 
                <div class="social-icon"> 
                <div class="social-item"> 
                <a href="#"><img src="https://img.icons8.com/bubbles/100/000000/facebook-new.png"></a> 
                </div> 
                <div class="social-item"> 
                <a href="#"><img src="https://img.icons8.com/bubbles/100/000000/instagram-new.png"></a> 
                </div> 
                <div class="social-item"> 
                <a href="#"><img src="https://img.icons8.com/bubbles/100/000000/twitter.png"></a> 
                </div> 
                <div class="social-item"> 
                <a href="#"><img src="https://img.icons8.com/bubbles/100/000000/behance.png"></a> 
                </div> 
                </div> 
                <p>Copyright © 2021 Element's™ ©. All rights reserved</p> 
                <p>&copy;Elements</p>
            </div> 
            </div>
    </div>
   
</template>
<script>
export default {
    name: 'Welcome',
    props: {
    msg: String
  }
}
</script>

<style scoped>
   h1{
       font-size: 35px;
       font-style: inherit;
       color: black;
       font-weight: 600;
   }p{
       font-size: 20px;
       font-style: inherit;
       font-weight: 400;
       color: #333;
   }
</style>