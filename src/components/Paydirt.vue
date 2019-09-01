<template>
    <div class="paydirt">

               
                <div class="p">
                <div v-for="part in p" 
                     :key="part.id"
                     :class="part.class"
                     :style="part.style"></div>
                </div>

                <div class="a">
                    <div v-for="part in a"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>        

                <div class="y">
                    <div v-for="part in y"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>

                 <div class="d">
                    <div v-for="part in d"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>

                
                 <div class="i">
                    <div v-for="part in i"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>

                <div class="r">
                    <div v-for="part in r"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>

                <div class="t">
                    <div v-for="part in t"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>
    </div>            
</template>

<script>
export default {
    name: "PayDirt",
    data(){
        return{
             p: [
                {
                id:0,
                class: "p-straight",
                style: {
                    position: "absolute",
                    height: "70px",
                    width: "20px",
                    backgroundColor: "#F0F8FD", 
                    }
                },
                {
                id:1,
                class: "p-top",
                style: {
                    position: "absolute",
                    height: "20px",
                    width: "35px",
                    backgroundColor: "#F0F8FD", 
                    }
                },
                {
                id:2,
                class: "p-bottom",
                style: {
                    position: "absolute",
                    height: "20px",
                    width: "35px",
                    backgroundColor: "#F0F8FD",
                    marginTop: "30px", 
                    }
                },
                {
                id:3,
                class: "p-curve",
                style: {
                    position: "absolute",
                    height: "50px",
                    width: "70px",
                    backgroundColor: "#F0F8FD",
                    borderRadius: "100%", 
                    }
                },
            ],
            a: [
                {
                id:0,
                class: "a-left",
                style: {
                    position: "absolute",
                    height: "50px",
                    width: "20px",
                    backgroundColor: "#F0F8FD", 
                    transform: "skew(-30deg)"
                    }
                },
                {
                id:1,
                class: "a-right",
                style: {
                    position: "absolute",
                    height: "50px",
                    width: "20px",
                    backgroundColor: "#F0F8FD",
                    transform: "skew(30deg)",
                    marginLeft: "28px", 
                    }
                },
                {
                id:2,
                class: "a-bottom",
                style: {
                    position: "absolute",
                    height: "17px",
                    width: "50px",
                    backgroundColor: "#F0F8FD",
                    marginTop: "30px",
                    marginLeft: "0px", 
                    }
                },
                
            ],

            y: [
                {id:0,
                class: "y-left",
                    style:{
                        position: "absolute",
                        height: "50px",
                        width: "23px",
                        backgroundColor: "#f0f8fd",
                        transform: "skew(10deg)",
                        marginLeft: "8px",
                    }
                },
               {id:1,
                class: "y-right",
                    style:{
                        position: "absolute",
                        height: "70px",
                        width: "25px",
                        backgroundColor: "#f0f8fd",
                        transform: "skew(-35deg)",
                        marginLeft: "23px",
                    }
                },
               
            ],

            d: [
                {id:0,
                class: "d-top",
                    style:{
                        position: "absolute",
                        height: "20px",
                        width: "35px",
                        backgroundColor: "#f0f8fd",
                    }
                },
               {id:1,
                class: "d-left",
                    style:{
                        position: "absolute",
                        height: "60px",
                        width: "20px",
                        backgroundColor: "#f0f8fd",
                    }
                },
                {id:2,
                class: "d-bottom",
                    style:{
                        position: "absolute",
                        height: "20px",
                        width: "35px",
                        backgroundColor: "#f0f8fd",
                        marginTop: "50px",
                    }
                },
                {id:3,
                class: "d-curve",
                    style:{
                        position: "absolute",
                        height: "70px",
                        width: "70px",
                        backgroundColor: "#f0f8fd",
                        borderRadius: "100%",
                    }
                },

            ],

            i: [
                {
                id:0,
                class: "i-rect",
                style: {
                    position: "absolute",
                    height: "55px",
                    width: "20px",
                    backgroundColor: "#f0f8fd",
                    marginLeft: "10px",
                    marginTop: "15px",
                    }
                }
            ],

            r: [
                {
                id:0,
                class: "r-left",
                style:{
                    position: "absolute",
                    height: "55px",
                    width: "20px",
                    backgroundColor: "#f0f8fd",
                    marginTop: "15px",
                    }
                },
                
                {
                 id:1,
                 class: "r-bottom",
                 style: {
                     position: "absolute",
                     height: "20px",
                     width: "40px",
                     backgroundColor: "#f0f8fd",
                     transform: "skew(70deg)",
                     marginTop: "50px",
                     marginLeft: "50px",
                 }    
                },

                {
                id:2,
                class: "r-curve",
                style: {
                    position: "absolute",
                    height: "30px",
                    width: "70px",
                    borderRight: "26px solid #f0f8fd",
                    marginTop: "15px",
                    borderRadius: "100%",
                }    
                }
            ],
            t: [
                {
                id:0,
                class: "t-top",
                style:{
                    position: "absolute",
                    height: "20px",
                    width: "90px",
                    backgroundColor: "#f0f8fd",
                    marginTop: "15px",
                    marginLeft: "10px",
                    }
                },
                
                {
                 id:1,
                 class: "t-bottom",
                 style: {
                     position: "absolute",
                     height: "55px",
                     width: "35px",
                     backgroundColor: "#f0f8fd",
                     marginTop: "15px",
                     marginLeft: "37px",
                 }    
                },
            ],

        }
    }
}
</script>

<style>
    /*Logo Positioning*/
    .paydirt{
        position: relative;
        display: grid;
        width: 500px;
        height: 70px;
        margin-top: 15vh;
        margin-left: auto;
        margin-right: auto;
        grid-template-columns: 
            repeat(6, 14.3%);
        grid-template-areas:
            "p a y d i r t";
        z-index: 5;
    }	

    .p{
    grid-area: p;
    }

    .a{    
    grid-area: a;
    margin-top: 20px;
    margin-left: 5px;    
    }

    .y{
    grid-area:y;
    margin-top: 17px;
    margin-left: -7px    
    }

    .d{
    grid-area: d;
    }

    .i{
        grid-area: i;
    }

    .r{
    grid-area: r;
    margin-left: -20px;
    }

    .t{
    grid-area: t;
    }

    

</style>
    