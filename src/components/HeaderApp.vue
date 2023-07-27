<script>
    export default {
  data() {
    return {
      count: 0
    }
  }
}
</script>


<template>
    <header>
        <div class="container">
            <div class="header-container">
                <div>
                    <img src="../assets/img/dark-logo.png" alt="">
                </div>

                <div class="nav">
                    <div>
                        <ul>
                            <li>
                                <a href="">
                                    Home
                                    <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                    Pages
                                    <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                   Courses 
                                   <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                   Features 
                                   <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                    Blog
                                    <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                    Shop
                                    <i class="fa-solid fa-chevron-down"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                    <i class="fa-solid fa-cart-shopping"></i>
                                </a>
                            </li>

                            <li>
                                <a href="">
                                    <i class="fa-regular fa-circle-user"></i>
                                </a>
                            </li>

                        </ul>
                    </div>

                    <div>
                        <input type="text" placeholder="Search...">
                    </div>
                </div>
            </div>
        </div>
    </header>

    <section>
        <div class="container">
            <div class="jumbo">

                <div class="jumbo-left">
                    <h2>
                        Complete Your Dreams in JavaS Programming
                    </h2>

                    <p>
                        Learn any coding program in distance and for a resonable fee. You don't have to struggle alone, you've got our assistance help
                    </p>

                    <button>
                        <i class="fa-solid fa-download"></i> Download free E-book
                    </button>
                </div>


                <div class="jumbo-right">
                    <img src="../assets/img/home-5-hero-image-279x300.png" alt="">
                </div>
            </div>
        </div>
    </section>
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

    header{
        height: 80px;
        background-color: $avorio;

       .header-container{
        display: flex;
        justify-content: space-between;
        align-items: center;

        img{
            height: 20px;
        }

        .nav{
            display: flex;
            align-items: center;

            ul{
                list-style: none;
                display: flex;

                li{
                    padding: 10px;

                    a{
                        text-decoration: none;
                    }
                }
            }
        }
       }
    }

    section{
        background-color: $grigio-chiaro;
        background-image: url('../assets/img/jumbo-overlay.svg');
        .jumbo{
        display: flex;
        align-items: center;

        .jumbo-left{
            width: 30%;

            h2, p{
                padding-right: 150px;
                padding-bottom: 20px;
                color: $viola;
            }

            p{
                font-size: 0.75em;
                color: $grigio-scuro;
            }

            button{
                padding: 15px;
                border-radius: 3px;
                background-color: $verde-acqua;
                border-color: $verde-acqua;
                color: $bianco;

                    button:hover{
                        background-color: $viola;
                    }

            }

            button:hover{
                        background-color: $viola;
                    }

            

            
        }

        .jumbo-right{
            width: 70%;

            img{
                padding-left: 210px;
            }
        }
        
    }
    }

</style>