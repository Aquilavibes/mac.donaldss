<template>
  
  <Navbar>
    <nav id='navy'>
      <img src='./assets/menu.png' id='menu'>
      <img src='./assets/mac-logo.png' id='logo'>
      <img src='./assets/search.png' id='search'>
      </nav>
  </Navbar>
  <br>
  <br>
  <img src='./assets/disount.jpg' id='dicount-img'>
  <Items>
    <p id="popular">Popular Now</p>
    <hr>
    <div class="foods">
   
   <div class='mob-div'>
      <div id="divy">
    <img src="./assets/chicken.png" id="chicken">
    <h4 id="name">{{ food1 }}</h4>
    </div>
    <div id="divy2">
  <p id="price">$10.00</p>
      <button id="buy">buy</button>
    </div>
    </div>
<hr>

<div class='mob-div'>
<div id="divy">
    <img src="./assets/double.png" id="chicken">
    <h4 id="name">{{ food3 }}</h4>
    </div>
    <div id="divy2">
  <p id="price">$6.00</p>
      <button id="buy">buy</button>
    </div>
</div>
<hr>

<div class='mob-div'>
<div id="divy">
    <img src="./assets/dried.png" id="chicken">
    <h4 id="name">{{ food5 }}</h4>
    </div>
    <div id="divy2">
  <p id="price">$8.00</p>
      <button id="buy">buy</button>
    </div>
    <hr>
    </div>
    </div>
  </Items>

  <h3 id='more'> See More...</h3><br>
  <h1 id='free'>Free large Fries Now.<br> Even more fries Later.</h1>
  <p id='desc'>Download the McDonalds app and join MyMcDonalds Reward
     to get your free Large fries with $1 minimum purchase. *Plus, when you join
      MyMcDonalds Rewards, you start earning pointson every eligible order-points
      you can put towards more free food.
      
  </p>
<div class='gety'>
  <p id='get'>Get Free Fries On The App</p>
</div><br><br>
<div class='footy'>
  <footer>
   <p id='privacy'> Privacy (Updated) </p>

    <p id='foot-desc'>privacy notice  | terms & conditions | Accessibility</p>
    <p id='do-not'> Do not sell or share My personal information</p>
    <div class="pics-div">
    <img src='./assets/facebook.png' id='social'>
    <img src='./assets/insta.png' id='social-fb'>
    <img src='./assets/twitter.png' id='social'>
    <img src='./assets/pin.png' id='social'>
    </div>
    
     </footer>

</div>
  </template>

<script>
export default {
  data(){
    return {
      food1: 'Chicken & Chips',
      food3: 'Double Cheeseburger',
      food5: 'Egg Muffin'
    }
  },
}
</script>

<style scoped>

#do-not {
  text-align: center;
}

.pics-div {
display: flex;
justify-content: center;
justify-content: space-evenly;
}

  #social {
    width: 35px;
    height: 35px;
    margin-top: 20px;
  }

  #social-fb {
    width: 55px;
  }

footer {
  font-size: 19px;
  font-weight: bold;
  
}

#free {
  font-weight: bolder;
  font-size: 40px;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
}

  #desc {
    font-size: 25px;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-weight: bold;
  }

.gety {
background-color: rgba(255, 255, 0, 0.795);
border-radius: 10px;
width: 238px;
height: 50px;
}

#get {
font-size: 19px;
font-weight: bolder;

}

  #more {
  background-color: rgba(236, 236, 26, 0.788);
  text-align: center;
  color: black;
  width: 90px;
  height: 30px;
  text-align: center;
  margin-left: 150px;
  }
#divy2 {
display:flex;
}
#price {
margin-left: 150px;
font-size: 23px;
font-weight: bold;
}

#name {
  font-size: 19px;
}

#buy {
height: 30px;
width: 60px;
background-color: red;
color: white;
margin-left: 120px;

}
#divy {
display: flex;
justify-content: space-around;
margin-right: 110px;
}
#chicken {
height: 95px; 
border: solid black;
border-radius: 20px;
}

#popular {
font-size: 29px;
font-family: Arial, Helvetica, sans-serif;
}

#order {
  background-color:red;
  color: white;
  margin-left: 330px;
}

#menu {
  height: 30px;
  margin-top: 10px;
  
}

#logo {
  height: 55px;
  width: 60px;
  
}

#search {
  height: 30px;
  margin-top: 10px;
}

#navy {
  display: flex;
  justify-content: space-between;
  background-color: rgba(0,0,0,0.5);
}

#dicount-img {
  width: 349px;
  height: 230px;
  margin-left: 16px;
}

#privacy {
  text-align: center;
}

#foot-desc {
  text-align: center;
}

.footy {
  background-color: yellow;
  padding-top: 30px;
  border-top-right-radius: 50px;
   border-top-left-radius: 50px;
   width: 100%;
}



@media (min-width: 1000px) {
  #dicount-img {
    width: 1100px;
    margin-left: 100px;
    justify-content: center;
    height: 350px;
  }

  #popular {
    font-size: 50px;
font-family: Arial, Helvetica, sans-serif;
  }

  #divy {
    display: block;
  }

  #divy2 {
    display: flex;
  }

  hr {
    display: none;
  }

  #chicken {
height: 200px; 
border: solid white;
width: 350px;

}

.mob-div {
  border: solid black; 
  width: 400px;
  border-radius: 28px;
  height: 350px;

}

.foods {
  display: flex;
  gap: 40px;
}

#name {
   font-size: 25px;
   margin-left: 40px;
}

#buy {
  margin-bottom: 100px;
  height: 30px;
}

#price {
  font-size: 25px;
  margin-top: 13px;
}

footer {
  font-size: 22px;
}
}




</style>

