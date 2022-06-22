<template>
        <!-- Lien d'évitement -->
        <a class="evitement" href="#main_content">Aller au contenu</a>

        <header id="header" role="banner">

            <nav role="navigation" aria-label="Menu principal">
                <ul class="desktop_only">
                    <li>
                        <a href="#">Homme</a>
                    </li>
                    <li>
                        <a href="#">Femme</a>
                    </li>
                    <li>
                        <a href="#">Concept</a>
                    </li>
                </ul>
                <!-- Burger *PROVISOIRE* -->
                <img :src="require('@/assets/images/burger-white.svg')" :class="'mobile_only'"  :alt="'Icone du burger-menu'"/>
            </nav>
            <!-- Logo -->
            <img :src="require('@/assets/images/logo-white.svg')" :class="'logo'" :alt="'Logo de The Kooples'"/>
            <!-- Panier -->
            <a href="#popup1">
                <img :src="require('@/assets/images/icon-cart-white.svg')" :alt="'Icone du panier'"/>
            </a>
                <!-- Pop-up du panier *PROVISOIRE*, source : https://codepen.io/imprakash/pen/GgNMXO -->
                <div id="popup1" class="overlay">
                    <div class="popup">
                        <a class="close" href="#">&times;</a>
                         <p class="content">
                             Votre panier est vide.
                        </p>
                    </div>
                </div>

        </header>

        <main id="main_content" role="main">

            <section id="first_section">
                <!-- Titre -->
                <h1>Femme</h1>
                <!-- Lien -->
                <a class="button" href="#">Découvrir</a>
            </section><!-- !#first_section -->

            <section id="second_section">
                <!-- Titre -->
                <h2>Lorem ipsum dolor sit amet</h2>
                <!-- Texte -->
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed nisi nisl, egestas nec purus nec, faucibus iaculis lectus. Curabitur ut aliquet turpis. Donec eros leo, porta ac bibendum quis, tempus sed sapien. In a arcu condimentum, fermentum mauris a, varius nisi. Phasellus ac lacus lorem. Curabitur sed urna augue. Nam viverra et lorem nec dictum. Duis vitae erat ac lacus rutrum mollis. Maecenas nisl risus, suscipit in pretium eu, pretium nec eros. Curabitur accumsan turpis a justo posuere, sed malesuada mi tempus.</p>
                <!-- Lien -->
                <a class="button" href="#">Découvrir</a>
            </section><!-- !#second_section -->

            <section id="collections">
                <ul>
                    <!-- Collection FEMME -->
                    <li>
                        <a href="#">
                            <img :src="require('@/assets/images/robe.jpeg')" :alt="'Collection femme'"/>
                            <p>Collection Femme</p>
                        </a>
                    </li>
                    <!-- Collection Homme -->
                    <li>
                        <a href="#">
                            <img :src="require('@/assets/images/homme.jpeg')" :alt="'Collection homme'"/>
                            <p>Collection Homme</p>
                        </a>
                    </li>
                </ul>

            </section><!-- !#collection -->

            <section id="our_selection">
                <h2>Notre Séléction</h2>
                
                <!-- Version Desktop (Sans carrousel) -->
                <ul class="desktop_only">
                    <li>
                        <a href="#">
                            <div class="text">
                                <h3>T-shirt Homme</h3>
                                <p>70,00 €</p>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <div class="text">
                                <h3>T-shirt Homme</h3>
                                <p>70,00 €</p>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <div class="text">
                                <h3>T-shirt Homme</h3>
                                <p>70,00 €</p>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <div class="text">
                                <h3>T-shirt Homme</h3>
                                <p>70,00 €</p>
                            </div>
                        </a>
                    </li>
                </ul>

                <!-- Carrousel pour la version mobile *PROVISOIRE*, source : https://codepen.io/ancaspatariu/pen/WpQYOP -->
                <div class="carousel mobile_only">
                    <ul class="slides">
                    <input type="radio" name="radio-buttons" id="img-1" checked />
                    <li class="slide-container">
                        <div class="slide-image">
                            <img :src="require('@/assets/images/product1.jpeg')" :alt="'T-shirt homme'"/>
                            <ul class="text">
                                <li><h3>T-shirt Homme</h3></li>
                                <li><p>70,00 €</p></li>
                            </ul>
                        </div>
                        <div class="carousel-controls">
                        <label for="img-3" class="prev-slide">
                            <span>&lsaquo;</span>
                        </label>
                        <label for="img-2" class="next-slide">
                            <span>&rsaquo;</span>
                        </label>
                        </div>
                    </li>
                    <input type="radio" name="radio-buttons" id="img-2" />
                    <li class="slide-container">
                        <div class="slide-image">
                            <img :src="require('@/assets/images/product2.jpeg')" :alt="'T-shirt homme'"/>
                            <ul class="text">
                                <li><h3>T-shirt Homme</h3></li>
                                <li><p>70,00 €</p></li>
                            </ul>
                        </div>
                        <div class="carousel-controls">
                        <label for="img-1" class="prev-slide">
                            <span>&lsaquo;</span>
                        </label>
                        <label for="img-3" class="next-slide">
                            <span>&rsaquo;</span>
                        </label>
                        </div>
                    </li>
                    <input type="radio" name="radio-buttons" id="img-3" />
                    <li class="slide-container">
                        <div class="slide-image">
                            <img :src="require('@/assets/images/product3.jpeg')" :alt="'T-shirt homme'"/>
                            <ul class="text">
                                <li><h3>T-shirt Homme</h3></li>
                                <li><p>70,00 €</p></li>
                            </ul>
                        </div>
                        <div class="carousel-controls">
                        <label for="img-2" class="prev-slide">
                            <span>&lsaquo;</span>
                        </label>
                        <label for="img-4" class="next-slide">
                            <span>&rsaquo;</span>
                        </label>
                        </div>
                    </li>
                    <input type="radio" name="radio-buttons" id="img-4" />
                    <li class="slide-container">
                        <div class="slide-image">
                            <img :src="require('@/assets/images/product4.jpeg')" :alt="'T-shirt homme'"/>
                            <ul class="text">
                                <li><h3>T-shirt Homme</h3></li>
                                <li><p>70,00 €</p></li>
                            </ul>
                        </div>
                        <div class="carousel-controls">
                        <label for="img-3" class="prev-slide">
                            <span>&lsaquo;</span>
                        </label>
                        <label for="img-1" class="next-slide">
                            <span>&rsaquo;</span>
                        </label>
                        </div>
                    </li>
                    <div class="carousel-dots">
                        <label for="img-1" class="carousel-dot" id="img-dot-1"></label>
                        <label for="img-2" class="carousel-dot" id="img-dot-2"></label>
                        <label for="img-3" class="carousel-dot" id="img-dot-3"></label>
                        <label for="img-4" class="carousel-dot" id="img-dot-4"></label>
                    </div>
                    </ul>
                </div>

            </section><!-- !#our_selection -->
            
            <section id="about">

                <img :src="require('@/assets/images/store.jpeg')" :alt="'Photo de la boutique The Kooples'"/>
                <div>
                    <a class="button" href="#">Découvrir</a>
                </div>

            </section><!-- !#about -->

        </main>

        <footer role="contentinfo">

            <nav role="navigation">
                <ul>
                    <li>
                        <a href="#">Faq</a>
                    </li>
                    <li>
                        <a href="#">Mentions légales</a>
                    </li>
                    <li>
                        <a href="#">CGV</a>
                    </li>
                </ul>
            </nav>
            
        </footer>

</template>

<script>
export default {
    name: 'DefaultLayout',
    mounted() {
        // Code JS Custom
            // Rendre le Header "Sticky" (source : https://www.w3schools.com/howto/howto_js_sticky_header.asp)
            window.onscroll = function() {sticky_header()};
            // Get the header
            var header = document.getElementById("header");
            // Get the offset position of the navbar
            var sticky = header.offsetTop;

            // Add the sticky class to the header when you reach its scroll position. Remove "sticky" when you leave the scroll position
            function sticky_header() {
            if (window.pageYOffset > sticky) {
                header.classList.add("sticky");
            } else {
                header.classList.remove("sticky");
            }
            }

    }
}
</script>

<style lang="scss">
// Variables
    // Polices
    $primary_font: "Open Sans", sans-serif;
    // Couleurs
        // Blanc
        $white_clr : #ffffff;
        // Noir
        $black_clr : #000000;
        // Gris
        $grey_clr : #eeeeee;

// Vue Desktop
 // Header
 header {
    padding: 15px 40px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
    width: 100%;
    position: fixed;
    top: 0;
    nav {
        ul {
            display: flex;
            align-items: center;
            column-gap: 20px;
            li {
                color: $white_clr;
                font-size: 18px;
                font-weight: 700;
                text-transform: uppercase;
                transition: .4s;
                &:hover {
                transform: scale(1.2);
                }
            }
        }
    }
    // Logo
    .logo {
        justify-self: center;
        width: 220px;
    }
    // Icone panier
    a {
        justify-self: end;
        img {
        width: 30px;
        height: 30px;
        transition: .4s;
        &:hover {
        transform: scale(1.2);
        }
        }
    }
 }
 // Effets sur le Header au scroll
 .sticky {
        background-color: $white_clr;
        z-index: 1;
        box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.5);
        // Passer les sous éléments du Header du Blanc au Noir
        nav, img {
            filter : invert(100%);
        }
        // Icone Burger
        nav {
            img {
                filter: invert(0%);
            }
        }
 }

 // Main 
 main {
    #first_section {
        background-image: url("@/assets/images/femme.jpeg");
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        row-gap: 30px;
        // Titre
        h1 {
            font-family: $primary_font;
            color: $white_clr;
            font-size: 100px;
            font-weight: bold;
            text-transform: uppercase;
        }
        a {
            border: solid 1px $white_clr;
        }
    }
    #second_section {
        padding: 80px 0 70px 0;
        h2 {
            font-family: $primary_font;
            font-size: 24px;
            font-weight: 700;
            text-transform: uppercase;
            text-align: center;
        }
        p {
            margin: 30px auto;
            text-align: center;
            font-size: 13px;
            font-weight: 400;
            max-width: 50%;
        }
        a {
            display: table;
            margin: 0 auto;
            border: solid 1px $black_clr;
            color: $black_clr;
            &:hover {
                color: $white_clr;
                border: solid 1px $white_clr;
            }
        }
    }
    #collections {
        ul {
            display: grid;
            grid-template-columns: 1fr 1fr;
            column-gap: 10px;
            li {
                a {
                    img {
                        width: 100%;
                        height: 80vh;
                        object-fit: cover;
                        transition: .4s;
                        &:hover {
                            opacity: .7;
                        }
                    }
                    p {
                        margin-bottom: -70px;
                        position: relative;
                        bottom: 70px;
                        left: 40px;
                        color: $white_clr;
                        font-size: 22px;
                    }
                }
            }
        }
    }
    #our_selection {
        padding: 80px 0;
        h2 {
            text-transform: uppercase;
            font-weight: 700;
            font-size: 24px;
            display: flex;
            justify-content: center;
            margin-right: 935px;
        }
        ul {
            margin-top: 30px;
            display: flex;
            column-gap: 10px;
            justify-content: center;
            li {
                a {
                    transition: .4s;
                    .text {
                        position: relative;
                        top: 370px;
                        h3 {
                        font-weight: 700;
                        }
                    }
                }
            }
            li:nth-of-type(1) {
                a {
                    display: block;
                    background-image: url("@/assets/images/product1.jpeg");
                    background-position: center;
                    background-size: cover;
                    background-repeat: no-repeat;
                    height: 360px;
                    width: 280px;
                    transition: .4s;
                    &:hover {
                        background-image: url("@/assets/images/product5.jpeg");
                    }
                }
            }
            li:nth-of-type(2) {
                a {
                    display: block;
                    background-image: url("@/assets/images/product2.jpeg");
                    background-position: center;
                    background-size: cover;
                    background-repeat: no-repeat;
                    height: 360px;
                    width: 280px;
                    transition: .4s;
                    &:hover {
                        background-image: url("@/assets/images/product5.jpeg");
                    }
                }
            }
            li:nth-of-type(3) {
                a {
                    display: block;
                    background-image: url("@/assets/images/product3.jpeg");
                    background-position: center;
                    background-size: cover;
                    background-repeat: no-repeat;
                    height: 360px;
                    width: 280px;
                    transition: .4s;
                    &:hover {
                        background-image: url("@/assets/images/product5.jpeg");
                    }
                }
            }
            li:nth-of-type(4) {
                a {
                    display: block;
                    background-image: url("@/assets/images/product4.jpeg");
                    background-position: center;
                    background-size: cover;
                    background-repeat: no-repeat;
                    height: 360px;
                    width: 280px;
                    transition: .4s;
                    &:hover {
                        background-image: url("@/assets/images/product5.jpeg");
                    }
                }
            }
        }
    }
    #about {
        display: grid;
        grid-template-columns: 1fr 1fr;
        img {
            width: 100%;
            height: 80vh;
            object-fit: cover;
        }
        div {
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: $grey_clr;
            .button {
                border: solid 1px $black_clr;
                color: $black_clr;
                &:hover {
                    color: $white_clr;
                    border-color: $white_clr;
                } 
            }
        }
    }
 }

 footer {
    padding: 80px 0;
    background-color: $black_clr;
    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        column-gap: 40px;
        color: $white_clr;
        li {
            color: $white_clr;
            transition: .4s;
            &:hover {
                color: $grey_clr;
                transform: scale(1.2);
            }
        }
    }
 }

 // Boutons
 .button {
            font-family: $primary_font;
            color: $white_clr;
            font-size: 20px;
            font-weight: 400;
            text-transform: uppercase;
            padding: 10px 50px;
            transition: .4s;
            &:hover {
                transform: scale(1.2);
                background-color: rgba(0,0,0,0.6);
            }
 }

 // Lien d'évitement (accessibilité)
 a.evitement {
    display: inline-block;
    color: #555;
    background: #fff;
    padding: .5em;
    position: absolute;
    left: -99999rem;
    z-index: 100;
 }
 a.evitement:focus {
    left: 0;
 }

// Overflow (*PROVISOIRE*, Causé par le Layout de Vue?)
html {
    overflow-x: hidden;
}
// Masquage de la version Mobile des produits (*PROVISOIRE*)
.mobile_only {
    display: none !important;
}

// Code externe
 // Pop-up au clique sur le panier ( *PROVISOIRE*, code source : https://codepen.io/imprakash/pen/GgNMXO )
 .box {
  width: 40%;
  margin: 0 auto;
  background: rgba(255,255,255,0.2);
  padding: 35px;
  border: 2px solid #fff;
  border-radius: 20px/50px;
  background-clip: padding-box;
  text-align: center;
}

.overlay {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.7);
  transition: opacity 500ms;
  visibility: hidden;
  opacity: 0;
}
.overlay:target {
  visibility: visible;
  opacity: 1;
}

.popup {
  margin: 70px auto;
  padding: 20px;
  background: #fff;
  border-radius: 5px;
  width: 30%;
  position: relative;
  transition: all 5s ease-in-out;
}

.popup .close {
  position: absolute;
  top: 5px;
  right: 30px;
  transition: all 200ms;
  font-size: 30px;
  font-weight: bold;
  text-decoration: none;
  color: #333;
}
.popup .close:hover {
  color: #06D85F;
}
.popup .content {
  max-height: 30%;
  overflow: auto;
}

// Vue Tablette
@media screen and (min-width: 577px) and (max-width: 992px){
    // Supression de l'overflow de la div "#app" de vue.js *PROVISOIRE* 
    #app {
        overflow: hidden;
    }

header {
    nav {
        ul {
            flex-direction: column;
            align-items: flex-start;
            column-gap: 0;
            row-gap: 10px;
        }
    }
}

main {
    #second_section {
        p {
            max-width: 70%;
        }
    }
    #collections {
        ul {
            li {
                a {
                    img {
                        height: 35vh;
                    }
                }
            }
        }
    }
    #our_selection {
        h2 {
            display: block;
            margin-right: 0;
            text-align: center;
        }
        ul {
            display: grid;
            grid-template-columns: 360px 360px;
            margin-left: auto;
            margin-right: auto;
            max-width: calc((360px*2) + 10px);
            row-gap: 80px;
            li {
                a {
                    margin: auto;
                }
            }
        }
    }
    #about {
        img {
            height: 35vh;
        }
    }
}

// Code externe
    //Pop-up au clique sur l'icone du panier (*PROVISOIRE*)
      .box{
            width: 70%;
        }
        .popup{
            width: 70%;
        }
}

// Vue Mobile
@media screen and (max-width: 576px){
 header {
    padding: 20px 15px;
}
main {
    #first_section {
        h1 {
            font-size: 78px;
        }
    }
    #second_section {
       h2 {
        font-size: 20px;
       }
       p {
        max-width: 70%;
       }
    }
    #collections {
        ul {
            display: block;
            li {
                a {
                    img {
                        height: 50vh;
                    }
                }
            }
            li:nth-of-type(2) {
                margin-top: 50px;
            }
        }
    }
    #our_selection {
        h2 {
            display: block;
            margin-right: 0;
            text-align: center;
            font-size: 20px;
        }
        ul {
            display: block;
            margin-left: auto;
            margin-right: auto;
            max-width: 100%;
            row-gap: 0px;
            li {
                img {
                    object-fit: cover;
                }
            }
        }
    }
    #about {
        display: block;
        background-color: $grey_clr;
        img {
            height: 50vh;
        }
        div {
            height: 50vh;
        }
    }
}

 // Masquage de la version desktop des produits (*PROVISOIRE*)
.desktop_only {
    display: none !important;
}
.mobile_only {
    display: block !important;
}

// Code externe
// Popup au clique sur le panier (*PROVISOIRE*)
 #app {
        overflow: hidden;
    }
    .box{
    width: 70%;
  }
  .popup{
    width: 70%;
  }
}

// Carrousel (*PROVISOIRE*)
ul.slides {
    display: block;
    position: relative;
    height: 500px;
    margin: 0;
    padding: 0;
    overflow: hidden;
    list-style: none;
}

.slides * {
    user-select: none;
    -ms-user-select: none;
    -moz-user-select: none;
    -khtml-user-select: none;
    -webkit-user-select: none;
    -webkit-touch-callout: none;
}

ul.slides input {
    display: none; 
}


.slide-container { 
    display: block; 
}

.slide-image {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    opacity: 0;
    transition: all .7s ease-in-out;
    object-fit: cover;
        .text {
        position: relative;
        bottom: 500px;
        left: 20px;
        h3 {
        font-weight: 700;
        }
    }
}   

.slide-image img {
    width: auto;
    min-width: 100%;
    height: 100%;
}

.carousel-controls {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    z-index: 999;
    font-size: 100px;
    line-height: 600px;
    color: #fff;
}

.carousel-controls label {
    display: none;
    position: absolute;
    padding: 0 20px;
    opacity: 0;
    transition: opacity .2s;
    cursor: pointer;
}

.slide-image:hover + .carousel-controls label{
    opacity: 0.5;
}

.carousel-controls label:hover {
    opacity: 1;
}

.carousel-controls .prev-slide {
    width: 49%;
    text-align: left;
    left: 0;
}

.carousel-controls .next-slide {
    width: 49%;
    text-align: right;
    right: 0;
}

.carousel-dots {
    position: absolute;
    left: 0;
    right: 0;
    bottom: 20px;
    z-index: 999;
    text-align: center;
}

.carousel-dots .carousel-dot {
    display: inline-block;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    background-color: #fff;
    opacity: 0.5;
    margin: 10px;
}

input:checked + .slide-container .slide-image {
    opacity: 1;
    transform: scale(1);
    transition: opacity 1s ease-in-out;
}

input:checked + .slide-container .carousel-controls label {
     display: block; 
}

input#img-1:checked ~ .carousel-dots label#img-dot-1,
input#img-2:checked ~ .carousel-dots label#img-dot-2,
input#img-3:checked ~ .carousel-dots label#img-dot-3,
input#img-4:checked ~ .carousel-dots label#img-dot-4,
input#img-5:checked ~ .carousel-dots label#img-dot-5,
input#img-6:checked ~ .carousel-dots label#img-dot-6 {
	opacity: 1;
}


input:checked + .slide-container .nav label { display: block; }
</style>