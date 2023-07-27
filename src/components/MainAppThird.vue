<script>
    export default {
  data() {
    return {
      events: [
        {
            location: 'Texas, US',
            nameEvent: 'Storytelling Workshop',
            day: '22',
            month: 'NOV',
        },
        {
            location: 'New York, US',
            nameEvent: 'Painting Art Contest 2020',
            day: '10',
            month: 'OCT',
        },
        {
            location: 'Hamburg, Germany',
            nameEvent: 'International Art Fair 2020',
            day: '23',
            month: 'NOV',
        },
        {
            location: 'Illinois, US',
            nameEvent: 'Street Performance: Call for Artist',
            day: '15',
            month: 'DEC',
        },
        {
            location: 'Illinois, US',
            nameEvent: 'Consumer Food Safety Education Conference',
            day: '22',
            month: 'JUL',
        },
        {
            location: 'Dubai',
            nameEvent: 'How Meditation improve you menthal health?',
            day: '12',
            month: 'AUG',
        }

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
                    GET IN CONTACT NOW
                </h4>
                <h3>
                    <strong>
                        Upcoming
                    </strong>
                    Events
                </h3>

                <div class="cards-container">
                    <div class="card" v-for="singleEvent in events">
                        <div>
                            <h5>
                                <i class="fa-solid fa-location-dot"></i>
                                {{ singleEvent.location }}
                            </h5>

                            <h4>
                                <strong>
                                    {{ singleEvent.nameEvent }}
                                </strong>
                            </h4>
                        </div>

                        <div class="date">
                            <h3>
                                {{ singleEvent.day }}
                            </h3>

                            <h4>
                                {{ singleEvent.month }}
                            </h4>

                            <div>
                                <button>
                                    Get ticket
                                </button>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="all-events">
                    <p>
                        Exited about our event?
                        <strong>
                            <a href="">
                                View all events 
                            </a>
                        </strong>
                    </p>
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
            background-color: $bianco;

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
            .cards-container{
                display: flex;
                flex-wrap: wrap;
                    .card{
                        display: flex;
                        justify-content: space-between;
                        width: calc((100% - 20px) / 2);
                        margin-right: 10px;
                        border: 1px solid $avorio;
                        background-color: $avorio;
                        margin-bottom: 20px;
                        padding-bottom: 10px;
                        padding-right: 5px;
                        
                            h5{
                                color: $grigio-scuro;
                                padding: 10px;
                            }
                            h4{
                                color: $viola;
                                padding: 10px;
                                font-size: 1.5em;
                                text-align: left;
                            }
                            .date{
                                h3{
                                    color: $verde-acqua;
                                    text-align: center;
                                    padding: 0%;

                                }
                                h4{
                                    color: $viola;
                                    text-align: center;
                                    font-size: 1em;
                                }
                                div{
                                    
                                        button{
                                            padding: 10px;
                                            background-color: $verde-acqua;
                                            color: $bianco;
                                            border-color: $verde-acqua;
                                            border-radius: 4px;
                                        }

                                        button:hover{
                                            background-color: $viola;
                                        }
               
                                } 
                            }
                    }
                    .card:hover{
                        background-color: $bianco-scuro;
                        border-left-color: $verde-acqua;
                    }
            }

            .all-events{
                padding: 20px;
                display: flex;
                justify-content: center;
                align-items: center;

                    p{
                        color: $grigio-scuro;
                            a{
                                color: $verde-acqua;
                                text-decoration: underline 1px solid $grigio-scuro;
                            }
                    }
            }
        }
}
</style>