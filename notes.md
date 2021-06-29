# Style Guide

## Layout

The designs were created to the following widths:

- Mobile:
- Desktop: 

## Header
background: #832833;
font-family: Prata;
### Nav bar
text color: #FFFFFF;

### Dana Fine Flowers
background: linear-gradient(180deg, #FFFFFF 0%, rgba(255, 255, 255, 0) 100%),
linear-gradient(0deg, #5E894A, #5E894A);

### carousel or slideshow
https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_slideshow

## Typography
font-family: Prata;
font-size: 64px;
font-style: normal;
font-weight: 400;
line-height: 87px;
letter-spacing: 0em;
text-align: left;


### Font(s)

- Family: [Prata](https://fonts.google.com/specimen/Prata?query=prata)
- Weights: 

- Family: [Prata](https://fonts.google.com/specimen/Prata?query=prata)
- Weights:

CSS
.photo__img {
  position: absolute;
  top: 0;
  left: 0;
  width: 70%;/*100%*/
  height: auto;/*100%*/
  object-fit:contain;/*scale-down*/
  border: 23px outset rgba(34, 34, 34, 0.2);
  margin-left:2rem;
}

.photo__gallery { (mobile)
    display: grid;
    grid-gap: .1px; 
    grid-template-columns:repeat(auto-fill,minmax(25%,1fr));
     
  } 
  .photo__gallery {
    display: grid;
    grid-gap: 5px; 
    grid-template-columns:repeat(3, 20%);
     
  } 

  WHOLE CODE:
  header {
    background-color: #832833;
    font-family: Prata;
    border-bottom: 1px solid #e2e8f0;
    display:flex;
    align-items: center;
  }
  header h1{
    margin-left: 4.2rem;
    font-size:2rem;
    color:#5E894A;
    text-shadow: 1px 2px 2px #d6e0d1;
  }
  /* navigation */
 .navbar {
   display:flex;
   justify-content: space-between;
   align-items: center;
   padding:1rem 1.5rem;
 }
 .hamburger {
  display: none;
}

.bar {
  display: block;
  width: 25px;
  height: 3px;
  margin: 5px auto;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
  background-color: #101010;
}

.nav-menu {
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.nav-item {
  margin-left: 1rem;
}

.nav-link{
  font-size:1.6rem;
  color:#FFFFFF;
}

.nav-link:hover{
  background-color:rgba(255, 255, 255, 0.5);
}
@media only screen and (max-width:768px) {
  .nav-menu {
    position: fixed;
    right:-100%; /*org. left:-100%*/
    top: 3rem;
    flex-direction: column;
    background-color: #832833;
    width: 100%;
    border-radius: 10px;
    text-align: center;
    transition:0.3s;
    box-shadow: 0 10px 27px rgba(0,0,0,0.05);
  }

  .nav-menu.active{
    right:0; /*org. left:0*/
  }
  .nav-item {
    margin: 2.5rem 0;
  }
  .hamburger {
    display: block;
    cursor: pointer;
  }
  .hamburger.active .bar:nth-child(2) {
    opacity: 0;
}

.hamburger.active .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
}

.hamburger.active .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
}
}

  .hero-flower {
    background:url(../img/hero.png);
    background-size: cover;
    background-position: center;
    min-height: 500px;
    display: flex;
    justify-content: center;
    flex-flow: row wrap;
  }

 .hero-flower h5{
  margin-top: 17rem;
  font-size:2rem;
  color:#CF3EA7;
  box-shadow:inset 22px 22px 22px rgba(255, 255, 255, 0.5);
  font-family: 'Princess Sofia', cursive;
  
 }
 .products h2{
  display:flex;
  justify-content: center;
  align-items: center;
  font-size:2rem;
  font-family: 'Princess Sofia', cursive;
  color:#5E894A;
  margin-top: 2rem;
}
.products h4 {
  display:flex;
  align-content: center;
  justify-content: center;
  margin: 1.5rem;
  color: #FFFFFF;
  font-size:2.3rem;
}
.products{
  display:grid;
  background-color:#C6CD5D;
  padding-bottom:100%;
}

.photo__gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  grid-gap: 455px;
}

.photo {
  position: relative;
  height: 0;
  padding-top: calc(3 / 5 * 100%);
}


.photo__img {
  position: absolute;
  top: 0;
  left: 0;
  width: 70%;/*100%*/
  height: auto;
  object-fit:contain;
  border: 23px outset rgba(34, 34, 34, 0.2);
  margin-left:2rem;
}

.photo h5{
  margin-top: 1.2rem;
 
}
.photo h5,
.photo p {
  display:flex;
  justify-content: center;
  align-items: center;
  font-size:1.5rem;
  
}

.photo p {
  line-height:1.8em;
}

.photo p a {
  color: #832833;

}

.prices {
  margin-top: 73%;
}
.prices p a {
  margin-top: -2.3%;
}

@media only screen and (min-width: 768px) {
 header{
   padding: 2%;
 }
  header h1{
    margin-left: 48%;
  }
  .nav-menu {
    top: 5rem;
  }

  .hero-flower h5 {
    font-size:4rem;
  }

  .photo__gallery {
    display: grid;
    grid-gap: 5px; 
    grid-template-columns:repeat(3, 1fr);
     
  } 
  .products h2{
    margin-bottom: 1rem;
  }
  .products h4 {
    margin:5%;
  
  }
  .products:nth-child(2) {
  padding-top:5%;
 
}

.products:nth-child(3),
.products:nth-child(4),
.products:nth-child(5) {
  margin-top:-50%;
}

}


@media only screen and (min-width: 1024px) {
.hero-flower h5 {
  font-size:5rem;
}

/* .products:nth-child(2) {
  padding-top:3%;

}

.products:nth-child(3),
.products:nth-child(4),
.products:nth-child(5) {
  margin-top:-60%;
} */

}


/* #contact figure img {
  padding-top:3%;
  width:50%;
} */

 