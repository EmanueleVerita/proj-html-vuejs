<script>
    export default {
  data() {
    return {
      testimonials: [
        {
            testimonialImage: '../assets/img/testimonial-avata-02.jpg',
            feedback: 'I am free to learn at my own place, follow my own schedule and choose the subject i like. Great study portal for people like me.',
            name: 'MINA HOLLACE',
            job: '/ Freelance'
        },
        {
            testimonialImage: '../assets/img/testimonial-avata-04.jpg',
            feedback: 'MaxCoach is my best choise. Their tutors are smart and professional when dealing whit students.',
            name: 'MADLEY PONDON',
            job: '/ IT Specialist'
        },
        {
            testimonialImage: '../assets/img/testimonial-avata-01.jpg',
            feedback: 'I am happy whit their arrangement of lesson and subject. They reflect a scientific investigation.',
            name: 'LUVIC DUBBLE',
            job: '/ Private Tutor'
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
                    PEOPLE ARE PRAISING MAXCOACHING
                </h4>
                <h3>
                    <strong>
                        What make they
                    </strong>
                    love us?
                </h3>

                <div class="feedback-container">
                    <div class="feedback" v-for="singleTestimonial in testimonials">
                        <div class="image-feedback">
                            <img :src="singleTestimonial.testimonialImage" alt="" class="circle-feedback-image">
                        </div>

                        <p>
                           {{ singleTestimonial.feedback }}
                        </p>

                        <h5>
                            {{ singleTestimonial.name }}
                        </h5>

                        <h6>
                            {{ singleTestimonial.job }}
                        </h6>
                    </div>

                </div>

                <div class="bottom-main">
                    <div>
                        <h4>
                        <strong>
                            Start today for getting 
                        </strong>
                        Online Certification
                    </h4>

                    <h3>
                        You can be your own guiding star whit our help!
                    </h3>

                    <div class="button-container">
                        <button>
                            Get started now
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

            .feedback-container{
                padding-top: 80px;
                display: flex;
                .feedback{
                    .image-feedback{
                        position: relative;
                        
                        .circle-feedback-image{
                            border-radius: 50%;
                            width: 100px;
                            height: 100px;
                            position: absolute;
                            top: - 50px;
                            left: 140px;
                            
                            
                        }
                    }
                    background-color: $avorio;
                    height: 200px;
                    width: calc((100% - 20px) / 3 );
                    margin: 10px;
                    border-radius: 4px;

                    p{
                        color: $viola;
                        text-align: center;
                        padding-top: 70px;
                        padding-bottom: 10px;
                    }

                    h5{
                        text-align: center;
                        font-size: 1.1em;
                        padding-bottom: 10px;
                    }

                    h6{
                        text-align: center;
                        color: $grigio-scuro;
                        font-size: 1.1em;
                    }
                }
            }
            .bottom-main{
                padding-top: 50px;
                display: flex;
                justify-content: center;
                align-items: center;
                background-image: url('../assets/img/maxcoach-shape-01.png'), url('../assets/img/maxcoach-shape-02.png');
                background-repeat: no-repeat;
                background-position: center left, bottom right;
                background-size: 70px, 70px;

                    h4{
                        color: $viola;
                            strong{
                                color: $verde-acqua;
                            }
                    }

                    h3{
                        color: $viola;
                        padding-bottom: 15px;
                        font-size: 1.25em;
                    }
                    .button-container{
                        display: flex;
                        justify-content: center;
                        button{
                            padding: 10px 30px;
                            background-color: $verde-acqua;
                            color: $bianco;
                            border-color: $verde-acqua;
                            border-radius: 4px;
                        }
                    }
                    
                
                
            }
    }
}
</style>