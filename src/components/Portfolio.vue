<template>
   <div>
   <div>
      <header>
       <div class="logo">
          <h5>ELEME<span>NTS</span> PORTFO<span>LIO</span>.</h5>
       </div>
       <nav>
                   <ul>
                        <li @click="toggleDetails" >
                        <svg xmlns="http://www.w3.org/2000/svg" width="18px" height="18px" fill="currentColor" class="bi bi-house-door-fill" viewBox="0 0 16 16">
                        <path d="M6.5 14.5v-3.505c0-.245.25-.495.5-.495h2c.25 0 .5.25.5.5v3.5a.5.5 0 0 0 .5.5h4a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4a.5.5 0 0 0 .5-.5z"/>
                        </svg><strong><a href="#">Home</a></strong>{{ home }}</li>
                        <li @click="toggleskill"><strong>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18px" height="18px" fill="currentColor" class="bi bi-gear-fill" viewBox="0 0 16 16">
                        <path d="M9.405 1.05c-.413-1.4-2.397-1.4-2.81 0l-.1.34a1.464 1.464 0 0 1-2.105.872l-.31-.17c-1.283-.698-2.686.705-1.987 1.987l.169.311c.446.82.023 1.841-.872 2.105l-.34.1c-1.4.413-1.4 2.397 0 2.81l.34.1a1.464 1.464 0 0 1 .872 2.105l-.17.31c-.698 1.283.705 2.686 1.987 1.987l.311-.169a1.464 1.464 0 0 1 2.105.872l.1.34c.413 1.4 2.397 1.4 2.81 0l.1-.34a1.464 1.464 0 0 1 2.105-.872l.31.17c1.283.698 2.686-.705 1.987-1.987l-.169-.311a1.464 1.464 0 0 1 .872-2.105l.34-.1c1.4-.413 1.4-2.397 0-2.81l-.34-.1a1.464 1.464 0 0 1-.872-2.105l.17-.31c.698-1.283-.705-2.686-1.987-1.987l-.311.169a1.464 1.464 0 0 1-2.105-.872l-.1-.34zM8 10.93a2.929 2.929 0 1 1 0-5.86 2.929 2.929 0 0 1 0 5.858z"/>
                        </svg><a href="#">Skill</a></strong>{{ skill }}</li>
                        <li @click="togglesproject"><strong>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18px" height="18px" fill="currentColor" class="bi bi-folder-fill" viewBox="0 0 16 16">
                        <path d="M9.828 3h3.982a2 2 0 0 1 1.992 2.181l-.637 7A2 2 0 0 1 13.174 14H2.825a2 2 0 0 1-1.991-1.819l-.637-7a1.99 1.99 0 0 1 .342-1.31L.5 3a2 2 0 0 1 2-2h3.672a2 2 0 0 1 1.414.586l.828.828A2 2 0 0 0 9.828 3zm-8.322.12C1.72 3.042 1.95 3 2.19 3h5.396l-.707-.707A1 1 0 0 0 6.172 2H2.5a1 1 0 0 0-1 .981l.006.139z"/>
                        </svg><a href="#">Projects</a></strong>{{ projects }}</li>
                        <li @click="toggleabout"><strong>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-person-circle" viewBox="0 0 16 16">
                        <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
                        <path fill-rule="evenodd" d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"/>
                        </svg><a href="#">About</a></strong>{{ about }}</li>
                        <li @click="togglecontacts"><strong>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-telephone-fill" viewBox="0 0 16 16">
                        <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"/>
                        </svg><a href="#">Contacts</a></strong>{{ contacts }}</li>
                     </ul>
       </nav>
      </header><br><br>
        <!-- Hero tagline & name -->
                    <div class="detail" v-if="detailsAreVisible">
                        <h1>Hello I'm Andrian <span>Elemento</span></h1>
                        <p><b>Life is just like proramming full of exploration, failure, mistakes and error <br>
                        but in every error's theres always solution to solve the problems and make it better</b></p>
                                
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

