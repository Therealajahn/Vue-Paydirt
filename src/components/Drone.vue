<template>
    <div class="drone">
        <div class="guard">
                    <div v-for="part in guard"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>
        <div class="curve">
                    <div v-for="part in curve"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>  
        <div class="spars">
                    <div v-for="part in spars"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>  
        <div class="cockpit">
                    <div v-for="part in cockpit"
                        :key="part.id"
                        :class="part.class"
                        :style="part.style"></div>
                </div>                    
    </div>
</template>

<script>
export default {
    name: "Drone",
    data(){
        return{
            guard: [
                {
                id:0,
                class: "guard1",
                style:{
                    position: "absolute",
                    height: "100px",
                    width: "100px",
                    border: "30px solid #000",
                    borderRadius: "50%",
                    }
                },
                
                {
                 id:1,
                 class: "guard2",
                 style: {
                     position: "absolute",
                     height: "100px",
                     width: "100px",
                     border: "30px solid #000",
                     borderRadius: "50%",
                     marginLeft: "170px",
                 }    
                },

                {
                id:2,
                class: "guard3",
                style: {
                    position: "absolute",
                    height: "100px",
                    width: "100px",
                    border: "30px solid #000",
                    borderRadius: "50%",
                    marginTop: "170px",
                    }    
                },

                {
                id:3,
                class: "guard4",
                style: {
                    position: "absolute",
                    height: "100px",
                    width: "100px",
                    border: "30px solid #000",
                    borderRadius: "50%",
                    marginTop: "170px",
                    marginLeft: "170px",
                    }    
                },
            ],

             curve: [
                {
                id:0,
                class: "curve1",
                style:{
                    position: "absolute",
                    height: "200px",
                    width: "50px",
                    borderBottom: "30px solid #000",
                    borderLeft: "12px solid transparent",
                    borderRight: "12px solid transparent",
                    borderRadius: "50%",
                    marginLeft: "128px",
                    marginTop: "-137px",
                    }
                },
                
                {
                 id:1,
                 class: "curve2",
                 style: {
                    position: "absolute",
                    height: "200px",
                    width: "50px",
                    borderBottom: "30px solid #000",
                    borderLeft: "12px solid transparent",
                    borderRight: "12px solid transparent",
                    borderRadius: "50%",
                    marginLeft: "318px",
                    marginTop: "50px",
                    transform: "rotate(90deg)",
                 }    
                },

                {
                id:2,
                class: "curve3",
                style: {
                    position: "absolute",
                    height: "200px",
                    width: "50px",
                    borderBottom: "30px solid #000",
                    borderLeft: "12px solid transparent",
                    borderRight: "12px solid transparent",
                    borderRadius: "50%",
                    marginLeft: "-62px",
                    marginTop: "50px",
                    transform: "rotate(-90deg)",
                    }    
                },

                {
                id:3,
                class: "curve4",
                style: {
                    position: "absolute",
                    height: "200px",
                    width: "50px",
                    borderBottom: "30px solid #000",
                    borderLeft: "12px solid transparent",
                    borderRight: "12px solid transparent",
                    borderRadius: "50%",
                    marginLeft: "128px",
                    marginTop: "239px",
                    transform: "rotate(180deg)",
                    }    
                },
            ],

            spars: [
                {
                id:0,
                class: "spar1",
                style:{
                   position: "absolute",
                   width: "20px",
                   height: "250px",
                   backgroundColor: "#67CAF5",
                   marginTop: "45px",
                   marginLeft: "150px",
                   transform: "rotate(45deg)",
                    }
                },
                
                {
                 id:1,
                 class: "spar2",
                 style: {
                   position: "absolute",
                   width: "20px",
                   height: "250px",
                   backgroundColor: "#67CAF5",
                   marginTop: "45px",
                   marginLeft: "160px",
                   transform: "rotate(-45deg)",
                 }    
                },

                {
                id:2,
                class: "spar-end1",
                style: {
                   position: "absolute",
                   width: "20px",
                   height: "20px",
                   borderRadius: "50%",
                   backgroundColor: "#67CAF5",
                   marginTop: "70px",
                   marginLeft: "70px",
                    }    
                },

                {
                id:3,
                class: "spar-end2",
                style: {
                   position: "absolute",
                   width: "20px",
                   height: "20px",
                   borderRadius: "50%",
                   backgroundColor: "#67CAF5",
                   marginTop: "70px",
                   marginLeft: "240px",
                    }    
                },

                {
                id:4,
                class: "spar-end3",
                style: {
                   position: "absolute",
                   width: "20px",
                   height: "20px",
                   borderRadius: "50%",
                   backgroundColor: "#67CAF5",
                   marginTop: "250px",
                   marginLeft: "60px",
                    }    
                },

                {
                id:5,
                class: "spar-end4",
                style: {
                   position: "absolute",
                   width: "20px",
                   height: "20px",
                   borderRadius: "50%",
                   backgroundColor: "#67CAF5",
                   marginTop: "250px",
                   marginLeft: "250px",
                    }    
                },

                {
                id:6,
                class: "spar-curve1",
                style: {
                   position: "absolute",
                   height: "200px",
                   width: "150px",
                   borderBottom: "15px solid #67CAF5",
                   borderLeft: "17px solid transparent",
                   borderRight: "17px solid transparent",
                   borderRadius: "50%",
                   marginTop: "-75px",
                   marginLeft: "72px", 
                    }    
                },

                {
                id:7,
                class: "spar-curve2",
                style: {
                   position: "absolute",
                   height: "200px",
                   width: "150px",
                   borderBottom: "15px solid #67CAF5",
                   borderLeft: "17px solid transparent",
                   borderRight: "17px solid transparent",
                   borderRadius: "50%",
                   marginTop: "57px",
                   marginLeft: "205px",
                   transform: "rotate(90deg)" 
                    }    
                },

                {
                id:8,
                class: "spar-curve3",
                style: {
                   position: "absolute",
                   height: "200px",
                   width: "150px",
                   borderBottom: "15px solid #67CAF5",
                   borderLeft: "17px solid transparent",
                   borderRight: "17px solid transparent",
                   borderRadius: "50%",
                   marginTop: "190px",
                   marginLeft: "73px",
                   transform: "rotate(180deg)" 
                    }    
                },

                {
                id:9,
                class: "spar-curve4",
                style: {
                   position: "absolute",
                   height: "200px",
                   width: "150px",
                   borderBottom: "15px solid #67CAF5",
                   borderLeft: "17px solid transparent",
                   borderRight: "17px solid transparent",
                   borderRadius: "50%",
                   marginTop: "58px",
                   marginLeft: "-60px",
                   transform: "rotate(-90deg)" 
                    }    
                },
            ],

            cockpit: [
                {
                id:0,
                class: "center",
                style:{
                    position: "absolute",
                    height: "150px",
                    width: "30px",
                    backgroundColor: "#69A4F3",
                    marginTop: "90px",
                    marginLeft: "150px",
                    }
                },
                
                {
                 id:1,
                 class: "left",
                 style: {
                     position: "absolute",
                     height: "90px",
                     width: "0px",
                     borderRight: "15px solid #347aef",
                     borderTop: "30px solid transparent",
                     borderBottom: "30px solid transparent",
                     marginTop: "90px",
                     marginLeft: "135px",
                 }    
                },

                 {
                 id:2,
                 class: "right",
                 style: {
                     position: "absolute",
                     height: "90px",
                     width: "0px",
                     borderLeft: "15px solid #347aef",
                     borderTop: "30px solid transparent",
                     borderBottom: "30px solid transparent",
                     marginTop: "90px",
                     marginLeft: "180px",
                 }    
                },
            ],
            
        }
    }
}
</script>

<style>
    /*Drone Positioning*/

.drone{
  height: 300px;
  width: 300px;    
  margin-top: -190px;
  margin-left: auto;
  margin-right: auto;
  z-index: 2;
}

.guard{
  margin-left:-16px;    
}

.curve{
    margin-left:-16px
}

.props{
  margin-left:-16px;    
}

.spars{
  margin-left:-16px;    
}

.cockpit{
  margin-left:-16px; 
}
</style>