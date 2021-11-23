<template>
  <div>
  <portfolio
            home=""
            skill=""
            projects=""
            about=""
            contacts=""
            Name=""
            MotherName=""
           Email=""
           Address=""
           Birthday=""
           GraduatedinElementary=""
           GraduatedinHighschool=""
           Working=""
        ></portfolio><br>
  <welcome msg="Welcome to Element's Personal Portfolio Website"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Portfolio from './components/Portfolio'
import Welcome from './components/Welcome'

export default {
  name: 'App',
  components: {
    // HelloWorld
       Portfolio,
       Welcome,
      
  },
  data() {
    return {
      contents: [ 
        { 
                      home: '',
                      skill: '',
                      projects: '',
                      about: '',
                      contacts: '',

                  },
                 ],
                 aboutme: [
                {
                  Name: 'Andrian Elemento O.',
                    MotherName: 'Leonisa Elemento',
                    FatherName: 'Vergilio Elemento',
                    Email: 'andri@gmail.com',
                    Address: 'Biton Magallanes Sorsogon',
                    Birthday: 'November 08, 1996',
                    GraduatedinElementary: 'Biton Elementary School',
                    GraduatedinHighschool: 'Biton National High School Batch: 2014-2015 from Old curiculum',
                    Working: 'As Fisherman',

                },
            ]
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
