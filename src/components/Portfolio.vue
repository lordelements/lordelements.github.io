<template>
   <div>
   <div>
      <header>
       <div class="logo">
          <h5>ELEME<span>NTS</span> PORTFO<span>LIO</span>.</h5>
       </div>
       <nav>
                   <ul>
                        <li @click="toggleDetails" ><strong><a href="#">Home</a></strong>{{ home }}</li>
                        <li @click="toggleskill"><strong><a href="#">Skill</a></strong>{{ skill }}</li>
                        <li @click="togglesproject"><strong><a href="#">Projects</a></strong>{{ projects }}</li>
                        <li @click="toggleabout"><strong><a href="#">About</a></strong>{{ about }}</li>
                        <li @click="togglecontacts"><strong><a href="#">Contacts</a></strong>{{ contacts }}</li>
                     </ul>
       </nav>
      </header><br><br>
        <!-- Hero tagline & name -->
                    <div class="detail" v-if="detailsAreVisible">
                        <h1>Hello I'm Andrian <span>Elemento</span></h1>
                        <p>Life is like proramming full of exploration and failure mistakes and error <br>
                        but in every error theres always solution to solve the problems and make it better</p>
                                
                        <br><button><a v-bind:href="ResumeLink" class="download-btn">Download Cv</a></button>
                    </div>

                     <!--  Skills  -->
          
                <div class="skill" v-if="skillsvisible">
                <section class="skill-container">
                    <h1>Skil<span>ls</span></h1>
                    <p class="text-1">This is the compilation of my recent projects
                        <br> and eperemints in previous and last semester</p>
                    
                    <div class="card">
                        <div class="icon"> 
                            <img src="https://img.icons8.com/bubbles/100/000000/services.png"> 
                        </div> 
                        <h2>C#</h2>
                                <p><br>In C# proramming language I've 
                                learned this when I'm first year student in college<br>
                                but C# language is hard to learned.
                            </p>
                    </div><br><br>

                        <div class="card">
                            <div class="icon"> 
                                <img src="https://img.icons8.com/bubbles/100/000000/services.png"> 
                            </div> 
                            <h2>PHP/MySQL</h2>
                               <p><br>In PHP/MySQL<br>
                                I've learned some basic of php&mysql in youtube from different 
                                programming and webdeveloper channel just like freecode camp tagalog tutorial <br>
                                I learned how to connect the php&MySQL in database and how to store a data.
                            </p>
                        </div><br><br>
                        
                        <div class="card">
                            <div class="icon"> 
                                <img src="https://img.icons8.com/bubbles/100/000000/services.png"> 
                            </div> 
                            <h2>HTML/CSS</h2>
                                    <p><br>This markup languge<br>
                                    is the most of all that I'm comfortable to learn because it more bit <br>
                                    easier that others, this frontend markup language that 
                                    I've to some youtube tutorial and to the module.
                                </p>
                        </div>
                  </section>
                </div><br><br>
               
                <!--  End of skills  -->

                <section>
     <!--  Projects   -->
                <div class="projects" v-if="projectsvisible">
                    <h1>Recent Proje<span>cts</span></h1><br>
                    <p class="text-1">This the compilation of my projects and eperemints in last lesson</p><br>
                    
                        <div class="card" >
                                <h2>Projects 1</h2><br>
                                <p><span><a v-bind:href="MonsterLink">Monster Slayer</a></span>
                                    <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                    Sint nam facilis commodi laudantium id sequi ipsam ab?
                                    Obcaecati ullam deleniti a dolorum dicta, vitae aperiam sit, aspernatur cum magnam aut!
                                </p>
                        </div><br><br>
                 <section>
                        <div class="card">
                            <h2>Projects 2</h2><br>
                            <p><span>Learning Resources App</span>
                                <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                Sint nam facilis commodi laudantium id sequi ipsam ab?
                                Obcaecati ullam deleniti a dolorum dicta, vitae aperiam sit, aspernatur cum magnam aut!
                            </p>
                        </div><br><br>

                        <div class="card">
                                <h2>Projects 3</h2><br>
                                <p><span>Find a coach web App</span>
                                    <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                    Sint nam facilis commodi laudantium id sequi ipsam ab?
                                    Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                                </p>
                        </div> <br><br>

                        <div class="card">
                            <h2>Projects 4</h2><br>
                            <p><span><a v-bind:href="ListandConditional">List and Conditional Statement</a></span>
                                <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                Sint nam facilis commodi laudantium id sequi ipsam ab?
                                Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                            </p>
                    </div>  <br><br>
                        
                            <div class="card">
                                <h2>Projects 5</h2><br>
                                <p><span><a href="#">Shopping Cart</a></span>
                                    <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                    Sint nam facilis commodi laudantium id sequi ipsam ab?
                                    Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                                </p>
                        </div> <br><br>
                        <div class="card">
                            <h2>Projects 6</h2><br>
                            <p><span>Sending Email Form</span>
                                <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                Sint nam facilis commodi laudantium id sequi ipsam ab?
                                Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                            </p>
                       </div> <br><br>
                       <div class="card">
                            <h2>Projects 7</h2><br>
                            <p><span><a v-bind:href="CrudLink">CRUD Using HTML,CSS/PHP,</a></span>
                                <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                Sint nam facilis commodi laudantium id sequi ipsam ab?
                                Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                            </p>
                       </div> <br><br>
                         <div class="card">
                            <h2>Projects 7</h2><br>
                            <p><span><a v-bind:href="LogInform">LogIn Form Using HTML,CSS/PHP,</a></span>
                                <br>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br>
                                Sint nam facilis commodi laudantium id sequi ipsam ab?
                                Obcaecati ullam deleniti a dolorum dicta,<br> vitae aperiam sit, aspernatur cum magnam aut!
                            </p>
                       </div> <br><br>
                       </section>
                </div>
                <!--  End of Projects  -->

                <!-- About Section --> 
            <section id="about" v-if="aboutvisible"> 
            <div class="about container"> 
                <div class="col-left"> 
                </div> 
                <div class="col-right"> 
                <h1 class="section-title">About <span>me</span></h1> 
                <h2>Hello I'm Andrian Elemento</h2> 
                <p>I'm I.T student of Sorsogon State University Bulan Campus</p> 

                <!-- About Me--> 
                <button @click="toggleDetailsinfo">Details</button>
                    <br><br>
                    <ul v-if="aboutmevisible">
                        <li>Name: {{  aboutme.Name }} </li>
                        <li>MotherName: {{  aboutme.MotherName }} </li>
                        <li>FatherName: {{ aboutme.FatherName }} </li>
                        <li>Email: {{ aboutme.Email }} </li>
                        <li>Address: {{ aboutme.Address }} </li>
                        <li>Birthday: {{ aboutme.Birthday }} </li>
                        <li>Graduated In Elementary: {{ aboutme.GraduatedinElementary }} </li>
                        <li>Graduated In High School: {{ aboutme.GraduatedinHighschool }} </li>
                        <li>Working: {{ aboutme.Working }} </li>
                    </ul>
                </div> 
            </div> 
            </section> 
            <!-- End About Section --> 
  <!-- Contact Section --> 
  <section id="contact" v-if="contactvisible"> 
        <div class="contact container"> 
            <div> 
            <h1 class="section-title">Contact <span>info</span></h1> 
            </div> 
            <div class="contact-items"> 
            <div class="contact-item"> 
            <div class="icon"> 
            <img src="https://img.icons8.com/bubbles/100/000000/phone.png"> 
            </div> 
            <div class="contact-info"> 
            
            <h2>+09109366801</h2> 
            <h2>+09973844979</h2> 
            </div> 
            </div> 
            <div class="contact-item"> 
            <div class="icon"> 
            <img src="https://img.icons8.com/bubbles/100/000000/new-post.png"> 
            </div> 
            <div class="contact-info"> 
            <h1>Email</h1> 
            <h2>elementoa@gmail.com</h2> 
            <h2>adrianelemento08@gmail.com</h2> 
            </div> 
            </div> 
            <div class="contact-item"> 
            <div class="icon"> 
            <img src="https://img.icons8.com/bubbles/100/000000/map-marker.png"> 
            </div> 
            <div class="contact-info"> 
            <h1>Address</h1> 
            <h2>Biton, Magallanes, Sorsogon</h2> 
            </div> 
            </div> 
            </div> 
        </div> 
  </section> 
  <!-- End Contact Section --> 
    </section>
        </div>
    </div>
    
</template>

    <script>
    
      export default {
      name: 'App',
//      components: {
     
//   },
  props: [
      'home',
      'skill',
      'projects',
      'about',
      'contacts'

  ],
         data() {
             return {
                 detailsAreVisible: false,
                 skillsvisible: false,
                 projectsvisible: false,
                 aboutvisible: false,
                 contactvisible: false,
                 aboutmevisible: false,
                 ResumeLink: 'https://drive.google.com/file/d/1Hvp9T70HnizwM-TreTd0YJ9nncVhEMj7/view?usp=sharing',
                 MonsterLink:'https://github.com/lordelements/Monster-Slayer-Game',
                 CrudLink: 'https://github.com/lordelements/crudapplication',
                 ListandConditional: 'https://github.com/lordelements/Lists-cond-assignment-problem',
                 LogInform: 'http://localhost/logIn/loginform.php',
                 
                  contents: {
                      home: '',
                      skill: '',
                      projects: '',
                      about: '',
                      contacts: '',

                  },
            aboutme:{
                    Name: 'Andrian Elemento O.',
                    MotherName: 'Leonisa Elemento',
                    FatherName: 'Vergilio Elemento',
                    Email: 'andri@gmail.com',
                    Address: 'Biton Magallanes Sorsogon',
                    Birthday: 'November 08, 1996',
                    GraduatedinElementary: 'Biton Elementary School',
                    GraduatedinHighschool: 'Biton National High School Batch: 2014-2015 from Old curiculum',
                    Working: 'As Fisherman',

            }
             };
         },
         methods: {
             toggleDetails() {
                 this.detailsAreVisible = !this.detailsAreVisible;
             },
             toggleskill() {
                 this.skillsvisible = !this.skillsvisible;
             },
             togglesproject() {
                this.projectsvisible = !this.projectsvisible;
            },
            toggleabout() {
                 this.aboutvisible = !this.aboutvisible;
             },
             togglecontacts() {
                 this.contactvisible = !this.contactvisible;
             },
             toggleDetailsinfo() {
                 this.aboutmevisible = !this.aboutmevisible;
             }
         }
      };
    </script>

