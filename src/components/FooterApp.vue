<script>
    export default {
  data() {
    return {
      
    }
  }
}
</script>


<template>
    <footer>
        <div class="container">
            <div class="footer-container">
                <div>
                <h4 class="address">
                    Address
                </h4>

                <p>
                    382 NE 191st St # 87394 Miami, FL 33179-3899
                </p>

                <p>
                    +1(305) 547-9909 (9am - 5pm EST, Monday - Fryday)
                </p>

                <p>
                    support@maxcoach.com
                </p>

                <h5>
                    <a href="">
                        <i class="fa-brands fa-square-facebook"></i>
                    </a> 
                    <a href="">
                        <i class="fa-brands fa-twitter"></i>
                    </a>
                    <a href="">
                        <i class="fa-brands fa-instagram"></i>
                    </a>
                    <a href="">
                        <i class="fa-brands fa-linkedin"></i>
                    </a>

                </h5>
            </div>

            <div class="footer-info">
                <div>
                    <h4>
                        Explore
                    </h4>

                    <ul>
                        <li>
                            <a href="">
                                Start here
                            </a>
                        </li>

                        <li>
                            <a href="">
                                Blog
                            </a>
                        </li>

                        <li>
                            <a href="">
                               About us 
                            </a>
                        </li>
                    </ul>
                </div>

                <div>
                    <ul class="contact-us">
                        <li>
                            <a href="">
                                Success story
                            </a>
                        </li>

                        <li>
                            <a href="">
                               Courses 
                            </a>
                        </li>

                        <li>
                            <a href="">
                                Contact us
                            </a>
                        </li>
                    </ul>
                </div>
               
                <div>
                    <h4 class="information">
                        Information
                    </h4>

                    <ul>
                        <li>
                            <a href="">
                                Membership
                            </a>
                        </li>

                        <li>
                            <a href="">
                                Purchase guide
                            </a>
                        </li>

                        <li>
                            <a href="">
                                Privacy policy
                            </a>
                        </li>

                        <li>
                            <a href="">
                               Terms of services 
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            </div>

                <div class="copyright">
                    <div>
                        <h5>
                            2020 Maxcoach All Rights Reserved
                        </h5>
                    </div>
                </div>
           
        </div>
    </footer>
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

    footer{
        .footer-container{
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 20px;

                .address{
                    padding-left: 10px;
                    padding-bottom: 20px;
                }

                p{
                    padding: 10px;
                }

                ul{
                    padding: 20px;
                }
                li{
                    list-style: none;
                    padding: 10px;
                }
                h5{
                    padding-left: 10px;
                    padding-top: 5px;
                   

                        i{
                            padding-right: 10px;
                            
                        }
                }
                a{
                    text-decoration: none;
                    color: $grigio-scuro;
                }
                .footer-info{
                    display: flex;
                    align-items: center;

                    h4{
                        padding-left: 30px;
                    }

                    .information{
                        padding-top: 35px;
                    }

                    .contact-us{
                        padding-top: 40px;
                    }
                }

                
        }
        .copyright{
                    margin: 20px;

                    h5{
                        text-align: center;
                        color: $grigio-scuro;
                    }
                }
    }
</style>