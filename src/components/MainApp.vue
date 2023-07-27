<script>
    export default {
  data() {
    return {
      courses: [
        {
            avatar: '../assets/img/home-5-image-box-01',
            courseType: 'Idea Discussion',
            description: 'Get teamed up with the specialists who work and teach coding for years at famous universities.'

        },
        {
            avatar: '../assets/img/home-5-image-box-02',
            courseType: 'Web Development',
            description: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.'

        },
        {
            avatar: '../assets/img/home-5-image-box-03',
            courseType: 'System Administration',
            description: 'Learners are encouraged to study the mechanism and structure of system administration.'

        },
        {
            avatar: '../assets/img/home-5-image-box-04',
            courseType: 'Graphic Design',
            description: 'Have a passion for graphic and arts? Show your talents with confidence and self-assertiveness.'

        }
      ]
    };
  },
  /*
  computed: {
    avatarImage(){
        return this.avatar;
    }
  }
  */
}
</script>


<template>
    <main>
        <section>
            <div class="container">

                <h4>
                    START LEARNING CODING NEW LANGUAGES
                </h4>
                <h3>
                    <strong>
                        Build You Dream
                    </strong>
                    TODAY
                </h3>

                <div class="courses-container">
                    <div  v-for="singleCourse in courses">
                        <img :src="singleCourse.avatar" alt="">

                       
                            <h4>
                                {{ singleCourse.courseType }}
                            </h4>

                            <p>
                                {{ singleCourse.description }}
                            </p>

                            <button>
                                Start now
                                <i class="fa-solid fa-arrow-right-long"></i>
                            </button>
                        
                    </div>
                
                </div>

            </div>
        </section>

        <section class="career-section">
            <div class="container">
                <div class="learning-types">
                    <div class="about-us-image">
                        <img src="../assets/img/about-us-03-image-01-215x300.png" alt="">
                    </div>


                    <div class="prospect-careers">
                        <h4>
                            DREAM WITH 
                            <strong>
                                MAXCOACH
                            </strong>
                        </h4>

                        <h3>
                            Costruct A 
                            <strong>
                                Stunning
                            </strong> 
                            Career Perspective
                        </h3>

                        <div class="boxes">
                            
                                <div class="opened-box">
                                    <h4>
                                        Multiple Platforms Supportated for Teaching & Studying
                                    </h4>
                                </div>

                                <div class="info-opened">
                                    <p>
                                        MaxCoach supports the act of teaching and learning on multiuple platforms like online or offline via material downloads. We know thigs aren't supposed to be devoured in a short time, you can always access our knowledge base from any devices.
                                    </p>
                                </div>
                            

                            <div class="box">
                                <h4>
                                    Multiple Course Participations at the Same Time 
                                </h4>
                            </div>

                            <div class="box">
                                <h4>
                                    Track Study Progress & Deliver Prompt Feedback
                                </h4>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="numbers-section">
            <div class="container">
                <div class="numbers-container">
                    <div>
                        <h3>
                            1.926
                        </h3>

                        <h4>
                            FINISHED SESSION
                        </h4>
                    </div>

                    <div>
                         <h3>
                            3.092+
                        </h3>

                        <h4>
                            ENROLLED LEARNES
                        </h4>
                    </div>

                    <div>
                         <h3>
                            200
                        </h3>

                        <h4>
                            ONLINE INSTRUCTORS
                        </h4>
                    </div>

                    <div>
                         <h3>
                            100%
                        </h3>

                        <h4>
                            SATISFACTION RATE
                        </h4>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>




<style lang="scss" scoped>
//COLORI

$bianco: #FFFFFF;
$verde-acqua: #20AD96;
$viola: #3F3A64;
$grigio-chiaro: #F5F7FA;
$avorio: #F8F8F8;
$bianco-scuro: #F5F1ED;
$grigio-scuro: #696969;
$grigio-viola: #8C89A2;

    main{
        section{
            padding: 20px;
            background-color: $bianco-scuro;

            h4{
                text-align: center;
                color:$grigio-scuro ;
                font-size: 0.75em;
            }

            h3{
                color: $verde-acqua;
                text-align: center;
                font-size: 2.5em;
                padding: 10px;

                strong{
                    color: $viola;
                }
            }
        }
        .courses-container{
            display: flex;
            div{
                width: calc(100% / 4);

                    img{
                        padding: 0 60px;
                    }
                
                    h4, p{
                        text-align: center;
                    }

                    h4{
                        font-size: 1.5em;
                        color: $viola;
                    }

                    p{
                        color: $grigio-scuro;
                        padding: 10px 0;
                    }

                    button{
                        background-color: $bianco-scuro;
                        color: $viola;
                        border: none;
                        padding: 10px;
                        margin: 0 90px;
                    }

                    button:hover{
                        color: $verde-acqua;
                    }
                
            }
        }

       .career-section{
        background-color: $bianco-scuro;
        .learning-types{
            display: flex;

            .about-us-image{
                width: 50%;
                display: flex;
                align-items: center;
                background-image: url('../assets/img/underlay-shape-lilla.svg');
                background-repeat: no-repeat;
                background-position: center;

                img{
                    padding-left: 180px;
                }
            }

            .prospect-careers{
                width: 50%;
                
                h4, h3{
                    text-align: left;
                    padding: 5px 0;
                }

                h4{
                    font-size: 1em;
                   
                }

                h3{
                    color: $viola;
                        strong{
                            color: $verde-acqua;
                        }
                }

                .boxes{
                    .opened-box{
                        border: 1px solid $bianco-scuro;
                        background-color: $verde-acqua;
                        border-radius: 4px;
                        padding: 10px;

                        

                            h4{
                                color: $bianco;
                            }
                        

                            
                    }

                    .info-opened{
                        background-color: $bianco;
                        border: 1px solid $avorio;
                        border-top: none;
                        border-radius: 4px;
                        margin-bottom: 5px;

                        p{
                                padding: 15px;
                                color: $grigio-scuro
                            }
                    }

                    .box{
                        border: 1px solid $bianco-scuro;
                        background-color: $bianco;
                        border-radius: 4px;
                        padding: 10px;
                        margin: 10px 0;

                        

                            h4{
                                color: $grigio-scuro;
                            }
                        
                    }
                }
            }
        }
       }
       .numbers-section{
        background-color: $avorio;
        .numbers-container{
            display: flex;

            div{
                width: calc(100% / 4);

                h3, h4{
                    text-align: center;
                }

                h3{
                    font-size: 1.75em;
                    color: $verde-acqua;
                }

                h4{
                    font-size: 0.75em;
                    color: $viola;
                }
            }
        }
       }
    }
</style>