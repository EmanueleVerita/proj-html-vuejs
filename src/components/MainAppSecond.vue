<script>
   export default {
  data() {
    return {
      achivments: [
        {
            image: '../assets/img/course-02-480x298.jpg',   
            circleImage: '../assets/img/73ee246daf47502812ccefc84bf02898.jpeg',
            name: 'Blanche Fields',
            achivment: 'Learning to Write as a Professional Author',
            numberLessons: '20 Lessons',
            numberStudents: '50 Students'
        },
        {
            image: '../assets/img/stock-full-hd-03-480x298.jpg',
            circleImage: '../assets/img/d0d504142acfde820eef2f11feea6253.jpeg',
            name: 'Maggie Strickland',
            achivment: 'Costumer-centric info-Tech Strategies',
            numberLessons: '24 Lessons',
            numberStudents: '769 Students'
        },
        {
            image: '../assets/img/stock-full-hd-04-480x298.jpg',
            circleImage: '../assets/img/d0d504142acfde820eef2f11feea6253.jpeg',
            name: 'Maggie Strickland',
            achivment: 'Open Programming Courses for Everyone: Python',
            numberLessons: '17 Lessons',
            numberStudents: '62 Students'
        },
        {
            image: '../assets/img/stock-full-hd-06-480x298.jpg',
            circleImage: '../assets/img/73ee246daf47502812ccefc84bf02898.jpeg',
            name: 'Blanche Fields',
            achivment: 'Academic Listening and Note-taking',
            numberLessons: '14 Lessons',
            numberStudents: '67 Students'
        },
        {
            image: '../assets/img/course-featured-image-01-480x298.jpg',
            circleImage: '../assets/img/73ee246daf47502812ccefc84bf02898.jpeg',
            name: 'Blanche Fields',
            achivment: 'Master jQuery in a Short Period of Time',
            numberLessons: '6 Lessons',
            numberStudents: '61 Students'
        },
        {
            image: '../assets/img/stock-full-hd-05-480x298.jpg',
            circleImage: '../assets/img/73ee246daf47502812ccefc84bf02898.jpeg',
            name: 'Blanche Fields',
            achivment: 'Introduction to Javascript for Beginners',
            numberLessons: '14 Lessons',
            numberStudents: '66 Students'
        },
      ]
    }
  }
}
</script>

<template>
      <main>
        <section>
            <div class="container">
                <h4>
                    CHOOSE WHERE YOU LIKE TO BEGIN
                </h4>
                <h3>
                    <strong>
                        Latest Featured
                    </strong>
                    Courses
                </h3>

                <div class="courses-achivment">
                   <div v-for="SingleAchivment in achivments">
                        <img :src="SingleAchivment.image" alt="" class="regular-image">
                        <div class="tutor">
                            <img :src="SingleAchivment.circleImage" alt="" class="circle-image">
                            <h4>
                                {{ SingleAchivment.name }}
                            </h4>
                        </div>

                        <h3>
                           {{ SingleAchivment.achivment }}
                        </h3>

                        <span class="lessons">
                            <i class="fa-regular fa-file-lines"></i> {{ SingleAchivment.numberLessons }}
                        </span>

                        <span class="students">
                            <i class="fa-regular fa-user"></i> {{ SingleAchivment.numberStudents }}
                        </span>
                   </div>

                </div>

                <div class="button-container">
                    <button>
                        View all courses <i class="fa-solid fa-arrow-right"></i>
                    </button>
                </div>
            </div>
        </section>

       

        <section class="learn-section">
            <div class="container">
                <div class="learn-container">
                    <div class="learn-info">
                        <h4>
                            WHY HESITATE TOREGISTER
                        </h4>
                        <h3>
                            <strong>
                               Learn At Your Own
                            </strong>
                            Pace
                        </h3>

                        <p>
                            <font-awesome-icon :icon="['fas', 'check']" />
                            Select & costumize courses to your preferences
                        </p>

                        <p>
                            <font-awesome-icon :icon="['fas', 'check']" />
                            Change the tutor and make arrangements
                        </p>

                        <p>
                            <font-awesome-icon :icon="['fas', 'check']" />
                            Posticipate in events to join others
                        </p>

                        <p>
                            <font-awesome-icon :icon="['fas', 'check']" />
                            Get the desired certificate delivered at house
                        </p>
                        <div>
                        <button>
                            Get started for free
                        </button>
                    </div>
                    </div>

                    <div class="learn-image">
                        <img src="../assets/img/home-5-image-01-269x300.png" alt="">
                    </div>
                    
                </div>
            </div>
        </section>

        <section class="learn-section">
            <div class="container">
                <div class="learn-container">

                    <div class="learn-mobile-image">
                        <img src="../assets/img/home-5-image-02-222x300.png" alt="">
                    </div>

                    <div class="learn-info">
                        <h4>
                            WHAT ARE YOU LOOKING FOR?
                        </h4>
                        <h3>
                            <strong>
                               Learn on your
                            </strong>
                                mobile
                            <strong>
                                anytime!
                            </strong>
                        </h3>

                        <p>
                           Save lessons for later and revise or write notes at any time and on multiple devices on your way. Never interfere with activities of enjoyment or other precious moments.
                        </p>

                        <div>
                            <button>
                                Download Our App
                            </button>
                        </div>

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
        .courses-achivment{
            display: flex;
            flex-wrap: wrap;
            margin-top: 15px;
            margin-bottom: 10px;

            div{
                width: calc( 100%   / 3);
                margin-bottom: 15px;

                .regular-image{
                    width: 350px;
                }
                

                .tutor{
                    display: flex;
                    padding-left: 10px;
                    padding-top: 5px;

                    .circle-image{
                        border-radius: 50%;
                        
                    }

                    h4{
                        color: $grigio-scuro;
                        padding-left: 5px;
                        padding-top: 7px;
                    }
                }

                h3{
                    font-size: 1.25em;
                    padding: 10px;
                    text-align: left;
                    color: $viola;
                }

                span{
                    color: $grigio-scuro;
                    padding: 10px;
                }
            }
        }
        .button-container{
            display: flex;
            justify-content: center;
            margin: 20px;

            button{
                padding: 10px 30px;
                background-color: $verde-acqua;
                color: $bianco;
                border-color: $verde-acqua;
                border-radius: 4px;
            }
        }

       .learn-section{
        background-color: $bianco;
        margin: 50px 0;
        .learn-container{
            display: flex;
            .learn-info{
                width: 50%;
                    h4{
                    text-align: left;
                    color:$grigio-scuro ;
                    font-size: 0.75em;
                    padding: 10px;
                }

                h3{
                    color: $verde-acqua;
                    text-align: left;
                    font-size: 2.5em;
                    padding: 10px;

                    strong{
                        color: $viola;
                    }
                }
                p{
                    color: $grigio-scuro;
                    padding: 10px;
                        i{
                            color: $verde-acqua;
                        }
                }
                div{
                    padding-left: 10px;
                    padding-top: 40px;
                        button{
                            padding: 10px 30px;
                            background-color: $verde-acqua;
                            color: $bianco;
                            border-color: $verde-acqua;
                            border-radius: 4px;
                        }
               
                }  
            }
            .learn-image{
                display: flex;
                justify-content: start;
                align-items: center;
                width: 50%;
                background-image: url('../assets/img/underlay-shape-grey.svg'), url('../assets/img/maxcoach-shape-05-100x100.png');
                background-repeat: no-repeat, no-repeat;
                background-position: left bottom, center;
                
            }  
            .learn-mobile-image{
                display: flex;
                justify-content: end;
                align-items: center;
                width: 50%;
                padding-right: 200px;
                background-image: url('../assets/img/underlay-shape-grey.svg'), url('../assets/img/maxcoach-shape-01.png'), url('../assets/img/maxcoach-shape-07-100x100.png');
                background-repeat: no-repeat, no-repeat, no-repeat;
                background-position: center bottom, center left, bottom right;
                background-size: 300px, auto, auto;
            }  
                    
        }
       }
}

</style>