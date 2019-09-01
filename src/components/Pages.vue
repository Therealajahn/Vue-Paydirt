<template>
        
        <div class="pages">    
        
        <div class="services-page">
            <div class="services-section1">
            <h1>Services</h1>
            </div>
            <div class="services-section2"></div>
            <div class="services-section3"></div>
            <div class="services-section4"></div>
            <div class="services-section5"></div>
        </div>
        
        <div class="people-page">
            <div class="people-section1">
            <h1>People</h1>
            </div>
            <div class="people-section2"></div>
            <div class="people-section3"></div>
            <div class="people-section4"></div>
            <div class="people-section5"></div>
        </div>    
        
        <div class="about-us-page">
            <div class="about-us-section1">
            <h1>About Us</h1>
            </div>
            <div class="about-us-section2"></div>
            <div class="about-us-section3"></div>
            <div class="about-us-section4"></div>
            <div class="about-us-section5"></div>    
        </div>
        
        <div class="contact-page">
            <div class="contact-section1">
            <h1>Contact</h1>
            </div>
            <div class="contact-section2"></div>
            <div class="contact-section3"></div>
            <div class="contact-section4"></div>
            <div class="contact-section5"></div>  
        </div>    
     </div>       
</template>

<script>
export default {
    name: "Pages",
    
}
</script>

<style>
    /*Pages Positioning*/

    .pages{
        height: 400vh;
        width: 100vw;
        display: grid;
        grid-template-rows: repeat(4, 100vh);
        grid-template-areas: 
            "services"
            "people"
            "about"
            "contact";
    }

    .services-page {
        grid-area: services;
        display: grid;
        background-color: #F0F8FD;
        grid-template-rows: repeat(5,20vh);
        grid-template-areas: 
            "section1"
            "section2"
            "section3"
            "section4"
            "section5";
    }

    .people-page {
        grid-area: people;
        display: grid;
        background-color: #F0F8FD;
        grid-template-rows: repeat(5,20vh);
        grid-template-areas: 
            "section1"
            "section2"
            "section3"
            "section4"
            "section5";
    }

    .about-us-page {
        grid-area: about;
        display: grid;
        background-color: #F0F8FD;
        grid-template-rows: repeat(5,20vh);
        grid-template-areas: 
            "section1"
            "section2"
            "section3"
            "section4"
            "section5";
    }

    .contact-page {
        grid-area: contact;
        display: grid;
        background-color: #F0F8FD;
        grid-template-rows: repeat(5,20vh);
        grid-template-areas: 
            "section1"
            "section2"
            "section3"
            "section4"
            "section5";
    }

    /*Pages*/

    /*SERVICES*/
    .services-section1{
        grid-area: section1;
        font-family: 'Lalezar', cursive;
        background-color: #1650DF;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .services-section1 > h1{
        margin-top: 20px
    }

    .services-section2{
        grid-area: section2;
        font-family: 'Lalezar', cursive;
        background-color: #4271ED;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .services-section3{
        grid-area: section3;
        font-family: 'Lalezar', cursive;
        background-color: #9EB6F6;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .services-section4{
        grid-area: section4;
        font-family: 'Lalezar', cursive;
        background-color: #C7D5FA;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .services-section5{
        grid-area: section5;
        font-family: 'Lalezar', cursive;
        background-color: #E9EEFD;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    /*PEOPLE*/
    .people-section1{
        grid-area: section1;
        font-family: 'Lalezar', cursive;
        background-color: #76D41A;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .people-section1 > h1{
        margin-top: 20px
    }

    .people-section2{
        grid-area: section2;
        font-family: 'Lalezar', cursive;
        background-color: #83E51D;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .people-section3{
        grid-area: section3;
        font-family: 'Lalezar', cursive;
        background-color: #93E83C;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .people-section4{
        grid-area: section4;
        font-family: 'Lalezar', cursive;
        background-color: #A4EB51;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .people-section5{
        grid-area: section5;
        font-family: 'Lalezar', cursive;
        background-color: #B4EE70;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    /*ABOUT US*/

    .about-us-section1{
        grid-area: section1;
        font-family: 'Lalezar', cursive;
        background-color: #3F09B9;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .about-us-section1 > h1{
        margin-top: 20px
    }

    .about-us-section2{
        grid-area: section2;
        font-family: 'Lalezar', cursive;
        background-color: #470AD7;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .about-us-section3{
        grid-area: section3;
        font-family: 'Lalezar', cursive;
        background-color: #4F0BEE;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .about-us-section4{
        grid-area: section4;
        font-family: 'Lalezar', cursive;
        background-color: #6A2EF6;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .about-us-section5{
        grid-area: section5;
        font-family: 'Lalezar', cursive;
        background-color: #8A58F8;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    /*CONTACT*/

    .contact-section1{
        grid-area: section1;
        font-family: 'Lalezar', cursive;
        background-color: #E51A7B;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .contact-section1 > h1{
        margin-top: 20px
    }

    .contact-section2{
        grid-area: section2;
        font-family: 'Lalezar', cursive;
        background-color: #E93F69;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .contact-section3{
        grid-area: section3;
        font-family: 'Lalezar', cursive;
        background-color: #ED6369;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .contact-section4{
        grid-area: section4;
        font-family: 'Lalezar', cursive;
        background-color: #F4817B;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

    .contact-section5{
        grid-area: section5;
        font-family: 'Lalezar', cursive;
        background-color: #F8A89C;
        text-align: center;
        letter-spacing: 40px;
        font-size: 30px;
        color: #F0F8FD;
    }

</style>