<template>
    <div class="intro-page">
    
    <div class="logo">    

        <Paydirt />
        <Drone />
    </div>

    <!--LINKS-->

        <div class="services-link" 
        :style="serviceStyle"> 
            
            <h1>Services</h1>
        </div>
        
        <div class="people-link"
        :style="peopleStyle"> 
            
            <h1>People</h1>
        </div>
        <div class="about-us-link"
        :style="aboutStyle"> 
            
            <h1>About Us</h1>
        </div>
        <div class="contact-link"
        :style="contactStyle"> 
            
            <h1>Contact</h1>
        </div>

    <!--Link Overlays-->
        
        <div class="services-over" 
        @mouseenter="servicesEnter()"
        @mouseout="servicesOut()"
        @click="servicesScroll()"
        ></div>
        
         <div class="over people-over" 
        @mouseenter="peopleEnter()"
        @mouseout="peopleOut()"
        @click="peopleScroll()"></div>
        
         <div class="over about-us-over" 
        @mouseenter="aboutEnter()"
        @mouseout="aboutOut()"
        @click="aboutScroll()"></div>
        
         <div class="over contact-over" 
        @mouseenter="contactEnter()"
        @mouseout="contactOut()"
        @click="contactScroll()"></div>

       <Pages />



    </div>
</template>

<script>


import Paydirt from "./Paydirt";
import Drone from "./Drone";
import Pages from "./Pages";

export default {
    name: "IntroPage",
    components: {
        Paydirt,
        Drone,
        Pages
    },
    methods: {
        
        //SERVICES
        servicesEnter() {
            this.serviceStyle.backgroundColor = "#0E3392";   
        },
        servicesOut() {
            this.serviceStyle.backgroundColor = "#1650DF";
        },
        servicesScroll() {
           
            window.scrollTo({
            top: window.innerHeight,
            left: 0,
            behavior: 'smooth'
        })
        },

         //PEOPLE
        peopleEnter() {
            this.peopleStyle.backgroundColor = "#4E8E12";   
        },
        peopleOut() {
            this.peopleStyle.backgroundColor = "#76D41A";
        },
        peopleScroll() {
           
            window.scrollTo({
            top: window.innerHeight * 2,
            left: 0,
            behavior: 'smooth'
        })
        },

         //ABOUT US
        aboutEnter() {
            this.aboutStyle.backgroundColor = "#280363";   
        },
        aboutOut() {
            this.aboutStyle.backgroundColor = "#3F09B9";
        },
        aboutScroll() {
            
            window.scrollTo({
            top: window.innerHeight * 3,
            left: 0,
            behavior: 'smooth'
        })
        },

         //CONTACT
        contactEnter() {
            this.contactStyle.backgroundColor = "#9C1153";   
        },
        contactOut() {
            this.contactStyle.backgroundColor = "#E51A7B";
        },
        contactScroll() {
           
            window.scrollTo({
            top: window.innerHeight * 4,
            left: 0,
            behavior: 'smooth'
        })
        },
    },
    
    data(){
        return{
            serviceStyle:{
                    gridArea: "services",
                    backgroundColor: "#1650DF",
                    fontFamily: "'Lalezar', cursive", 
                    fontSize: "16px",
                    letterSpacing: "20px",      
                    textAlign: "center",
                    color: "#F0F8FD",
                    zIndex: "-1", 
            },

            peopleStyle:{
                    gridArea: "people",
                    backgroundColor: "#76d41a",
                    fontFamily: "'Lalezar', cursive", 
                    fontSize: "16px",
                    letterSpacing: "20px",      
                    textAlign: "center",
                    color: "#F0F8FD",
                    zIndex: "-1", 
            },

            aboutStyle:{
                    gridArea: "about",
                    backgroundColor: "#3F09B9",
                    fontFamily: "'Lalezar', cursive", 
                    fontSize: "16px",
                    letterSpacing: "20px",      
                    textAlign: "center",
                    color: "#F0F8FD",
                    zIndex: "-1", 
            },

            contactStyle:{
                    gridArea: "contact",
                    backgroundColor: "#E62066",
                    fontFamily: "'Lalezar', cursive", 
                    fontSize: "16px",
                    letterSpacing: "20px",      
                    textAlign: "center",
                    color: "#F0F8FD",
                    zIndex: "-1", 
            },
        }
    }

}            
    


</script>

<style scoped>
    
.intro-page{
    display: grid;
    width: 100vw;
    height: 100vh;
    grid-template-rows: 25vh 45vh 30vh;
    grid-template-columns: 50vw 50vw;
    grid-template-areas:
        "services people"
        "logo logo"
        "about contact";
    font-family: "Lalezar", cursive;    
}
.logo{
  grid-area: logo;
  background-color: #125084;    
}

.services-link{
  grid-area: services;
  background-color: #1650DF;
  font-family: 'Lalezar', cursive; 
  font-size: 16px;
  letter-spacing: 20px;      
  text-align: center;
  color: #F0F8FD;
  z-index: -1; 
  font-family: "Lalezar", cursive; 
}


.people-link{
  grid-area: people;
  background-color: #76D41A;
  font-family: 'Lalezar', cursive;  font-size: 18px;
  letter-spacing: 30px;      
  text-align: center;
  color: #F9FCFE;
  z-index: -10;
}

.about-us-link{
  grid-area: about;
  background-color: #3F09B9;
  font-family: 'Lalezar', cursive; 
  font-weight: 700;  
  font-size: 18px;
  letter-spacing: 30px;      
  text-align: center;
  color: #F0F8FD;  
  z-index: -10;   
}

.contact-link{
  grid-area: contact;
  background-color: #E62066;
  font-family: 'Lalezar', cursive; 
  font-weight: 700;  
  font-size: 18px;
  letter-spacing: 30px;      
  text-align: center;
  color: #F0F8FD;
  z-index: -10;  
}

/*H1s + Overlays*/

.services-over{
	grid-area: services;

}

.people-over{
	grid-area: people;
}

.about-us-over{
	grid-area: about;
}

.contact-over{
	grid-area: contact;
}

.services-link > h1 {
    margin-top: 50px;
    margin-left: 5px;
}

.people-link > h1 {
    margin-top: 50px;
    margin-left: 20px
}

.about-us-link > h1 {
    margin-top: 70px;
    margin-left: 20px;
}

.contact-link > h1 {
    margin-top: 70px;
    margin-left: 20px;
}

.people-link > h1 {
    margin-top: 50px;
    margin-left: 20px
}

.about-us-link > h1 {
    margin-top: 70px;
    margin-left: 20px;
}

.contact-link > h1 {
    margin-top: 70px;
    margin-left: 20px;
}


</style>