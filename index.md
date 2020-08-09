<html>
  <head>
    <title id="title"> 0 Pokes </title>
    <style>
      body {
        background: url('https://i.pinimg.com/originals/0a/41/de/0a41de68578f5d87900c47932565c002.jpg') no-repeat center center fixed; 
        background-size: cover;
        font-family: monospace;
      }
      .wrapper {
       max-width:0
      }
      p {
        position: relative;
        z-index: 1;
        color: black
      }
      .entry {
        display: none;
        float: left;
        height: 200px;
        border: 1px solid black;
        margin: 2px;
        border-radius: 20px;
        text-align: center;
        background: #FCFCFC;
      }
      .oaktext {
        background-color: white;
        border: 1px solid black;
        border-radius: 10px;
      }
      .item {
        background-color: white;
        border: 1px solid black;
        border-radius: 10px;
        width: 110px;
        float: left;
      }
      .item button {
        width: 110px;
      }
      .aquatica {
        display: none;
      }
      .grid-container {
        display: grid;
        grid-template-columns: 33vw 33vw 33vw;
        grid-template-rows: 50vh 50vh;
      }
      .two, .four, .five {
        overflow: auto;
      }
      .one { grid-area: 1 / 1 / 2 / 2; }
      .two { grid-area: 2 / 1 / 3 / 2; }
      .three { grid-area: 1 / 2 / 3 / 3; }
      .four { grid-area: 1 / 3 / 2 / 4; }
      .five { grid-area: 2 / 3 / 3 / 4; }
    </style>
  </head>
  <body>
  <div class="grid-container">
    <div class="one">
      <button class="clicker" onclick="morepoke()" id="clicker" disabled>
        <img src="https://cdn.bulbagarden.net/upload/7/79/Dream_Pok%C3%A9_Ball_Sprite.png">
        <div id="pokesgot">0 Pokecoins</div>
      </button>
    </div>
    <div class="two">
      <div id="bulb" class="entry">
        <p>001</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/1.png">
        <p>Bulbasaur</p>
        <p id="bulbcount">0</p>
      </div>
      <div id="charm" class="entry">
        <p>004</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/4.png">
        <p>Charmander</p>
        <p id="charmcount">0</p>
      </div>
      <div id="squirt" class="entry">
        <p>007</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/7.png">
        <p>Squirtle</p>
        <p id="squirtcount">0</p>
      </div>
      <div id="cater" class="entry">
        <p>010</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/10.png">
        <p>Caterpie</p>
        <p id="catercount">0</p>
      </div>
      <div id="pidge" class="entry">
        <p>016</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/16.png">
        <p>Pidgey</p>
        <p id="pidgecount">0</p>
      </div>
      <div id="rat" class="entry">
        <p>019</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/19.png">
        <p>Rattata</p>
        <p id="ratcount">0</p>
      </div>
      <div id="nidogirl" class="entry">
        <p>029</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/29.png">
        <p>Nidoran F</p>
        <p id="nidogirlcount">0</p>
      </div>
      <div id="nidoboy" class="entry">
        <p>032</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/32.png">
        <p>Nidoran M</p>
        <p id="nidoboycount">0</p>
      </div>
      <div id="karp" class="entry">
        <p>129</p>
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/129.png">
        <p>Magikarp</p>
        <p id="karpcount">0</p>
      </div>
    </div>
    <div class="three">
      <div class="oak">
        <img src="https://i.pinimg.com/originals/84/04/3e/84043e578223f640f524332544a47eba.png">
        <div id="oaktext" class="oaktext">
        Hello there, and welcome to the world of Pokémon! My name is Proffesor Oak! This world is inhabited by creatures called Pokémon! For some people, Pokémon are pets. Others use them for fights...
        Your very own Pokémon adventure is about to unfold! A world of dreams and adventures with Pokémon awaits! Let's go!
        Now, please choose a starter Pokémon!
        <button onclick="bulbasaur()" class="starter">
          <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/1.png">
          <p>Bulbasaur</p>
        </button>
        <button onclick="charmander()" class="starter">
          <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/4.png">
          <p>Charmander</p>
        </button>
        <button onclick="squirtle()" class="starter">
          <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/7.png">
          <p>Squirtle</p>
        </button>
      </div>
    </div>
    </div>
    <div class="four">
      <div class="item" id="rattata">
        <p>Rattata</p>
        <p id="ratcoins">10 Pokecoins</p>
        <button class="buy" onclick="buyrattata()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/19.png">
        </button>
      </div>
      <div class="item" id="pidgey">
        <p>Pidgey</p>
        <p id="pidgecoins">25 Pokecoins</p>
        <button class="buy" onclick="buypidgey()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/16.png">
        </button>
      </div>
      <div class="item" id="nidorangirl">
        <p>Nidoran F</p>
        <p id="nidogirlcoins">45 Pokecoins</p>
        <button class="buy" onclick="buynidogirl()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/29.png">
        </button>
      </div>
      <div class="item" id="caterpie">
        <p>Caterpie</p>
        <p id="catercoins">60 Pokecoins</p>
        <button class="buy" onclick="buycater()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/10.png">
        </button>
      </div>
      <div class="item aquatica" id="magikarp">
        <p>Magikarp</p>
        <p id="karpcoins">75 Pokecoins</p>
        <button class="buy" onclick="buykarp()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/129.png">
        </button>
      </div>
      <div class="item" id="nidoranboy">
        <p>Nidoran M</p>
        <p id="nidoboycoins">100 Pokecoins</p>
        <button class="buy" onclick="buynidoboy()">
        <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/32.png">
        </button>
      </div>
    </div>
    <div class="five">
      <div class="item" id="oldrod">
        <p>Old Rod</p>
        <p>150 Pokecoins</p>
        <button class="buy" onclick="buyoldrod()" style="overflow: hidden;">
        <img src="https://cdn.bulbagarden.net/upload/thumb/e/e2/RG_Good_Rod.png/150px-RG_Good_Rod.png">
        </button>
        <p>Allows you to catch some aquatic Pokemon</p>
        <p id="gotoldrod">N</p>
      </div>
    </div>
   </div>
     <script>
      var gameData = {
      pokes: 0,
      totalpokes: 0,
      clicks: 0,
      pokesPerClick: 1,
      ratcost: 10,
      pidgecost: 25,
      nidogirlcost: 45,
      nidoboycost: 100,
      catercost: 60,
      karpcost: 75,
      bulb: 0,
      charm: 0,
      squirt: 0,
      rat: 0,
      pidge: 0,
      nidogirl: 0,
      nidoboy: 0,
      cater: 0,
      karp: 0
    }
    function morepoke() {
      gameData.pokes += gameData.pokesPerClick
      gameData.totalpokes += gameData.pokesPerClick
      gameData.clicks += 1
      document.getElementById("pokesgot").innerHTML = gameData.pokes + " Pokecoins"
      document.getElementById("title").innerHTML = gameData.pokes + " Pokecoins"
    }
    function bulbasaur() {
      gameData.bulb += 1
      setInterval(function(){ checker(); }, 1000);
      document.getElementById("oaktext").innerHTML = "Bulbasaur, the grass type Pokémon! A great choice! Now, try clicking on the pokeball to earn some pokecoins!"
      document.getElementById("clicker").disabled = false;
      document.getElementById('bulbcount').innerHTML = gameData.bulb
      var x = document.getElementsByClassName("starter");
      var i;
      for (i = 0; i < x.length; i++) {
        x[i].style.display = 'none';
      }
    }
    function charmander() {
      gameData.charm += 1
      setInterval(function(){ checker(); }, 1000);
      document.getElementById("oaktext").innerHTML = "Charmander, the fire type Pokémon! A great choice! Now, try clicking on the pokeball to earn some pokecoins!"
      document.getElementById("clicker").disabled = false;
      document.getElementById('charmcount').innerHTML = gameData.charm
      var x = document.getElementsByClassName("starter");
      var i;
      for (i = 0; i < x.length; i++) {
        x[i].style.display = 'none';
      }
    }
    function squirtle() {
      gameData.squirt += 1
      setInterval(function(){ checker(); }, 1000);
      document.getElementById("oaktext").innerHTML = "Squirtle, the water type Pokémon! A great choice! Now, try clicking on the pokeball to earn some pokecoins!"
      document.getElementById("clicker").disabled = false;
      document.getElementById('squirtcount').innerHTML = gameData.squirt
      var x = document.getElementsByClassName("starter");
      var i;
      for (i = 0; i < x.length; i++) {
        x[i].style.display = 'none';
      }
    }
    function buyrattata() {
      if (gameData.pokes >= gameData.ratcost) {
        gameData.pokes -= gameData.ratcost
        gameData.rat += 1
        gameData.ratcost *= 2
        document.getElementById('ratcoins').innerHTML = gameData.ratcost + " Pokecoins"
        document.getElementById('ratcount').innerHTML = gameData.rat
      }
    }
    function buypidgey() {
      if (gameData.pokes >= gameData.pidgecost) {
        gameData.pokes -= gameData.pidgecost
        gameData.pidge += 1
        gameData.pidgecost *= 2
        document.getElementById('pidgecoins').innerHTML = gameData.pidgecost + " Pokecoins"
        document.getElementById('pidgecount').innerHTML = gameData.pidge
      }
    }
    function buynidogirl() {
      if (gameData.pokes >= gameData.nidogirlcost) {
        gameData.pokes -= gameData.nidogirlcost
        gameData.nidogirl += 1
        gameData.nidogirlcost *= 2
        document.getElementById('nidogirlcoins').innerHTML = gameData.nidogirlcost + " Pokecoins"
        document.getElementById('nidogirlcount').innerHTML = gameData.nidogirl
      }
    }
    function buynidoboy() {
      if (gameData.pokes >= gameData.nidoboycost) {
        gameData.pokes -= gameData.nidoboycost
        gameData.nidoboy += 1
        gameData.nidoboycost *= 2
        document.getElementById('nidoboycoins').innerHTML = gameData.nidoboycost + " Pokecoins"
        document.getElementById('nidoboycount').innerHTML = gameData.nidoboy
      }
    }
    function buycater() {
      if (gameData.pokes >= gameData.catercost) {
        gameData.pokes -= gameData.catercost
        gameData.cater += 1
        gameData.catercost *= 2
        document.getElementById('catercoins').innerHTML = gameData.catercost + " Pokecoins"
        document.getElementById('catercount').innerHTML = gameData.cater
      }
    }
    function buykarp() {
      if (gameData.pokes >= gameData.karpcost) {
        gameData.pokes -= gameData.karpcost
        gameData.karp += 1
        gameData.karpcost *= 2
        document.getElementById('karpcoins').innerHTML = gameData.karpcost + " Pokecoins"
        document.getElementById('karpcount').innerHTML = gameData.karp
      }
    }
    function buyoldrod() {
      if (gameData.pokes >= 150) {
        gameData.pokes -= 150
        document.getElementById('gotoldrod').innerHTML = "Y"
        document.getElementById("oldrod").disabled = true;
        var x = document.getElementsByClassName("aquatica");
        var i;
        for (i = 0; i < x.length; i++) {
          x[i].style.display = 'inline';
        }
      }
    }
    function checker() {
      if (gameData.bulb >= 1) {
        document.getElementById('bulb').style.display = 'inline';
      }
      if (gameData.charm >= 1) {
        document.getElementById('charm').style.display = 'inline';
      }
      if (gameData.squirt >= 1) {
        document.getElementById('squirt').style.display = 'inline';
      }
      if (gameData.pidge >= 1) {
        document.getElementById('pidge').style.display = 'inline';
      }
      if (gameData.nidogirl >= 1) {
        document.getElementById('nidogirl').style.display = 'inline';
      }
      if (gameData.karp >= 1) {
        document.getElementById('karp').style.display = 'inline';
      }
      if (gameData.nidoboy >= 1) {
        document.getElementById('nidoboy').style.display = 'inline';
      }
      if (gameData.cater >= 1) {
        document.getElementById('cater').style.display = 'inline';
      }
      if (gameData.pokes >= 10) {
        document.getElementById('oaktext').innerHTML = "Great! Now you can use your pokecoins to catch a Pokémon! Catch a Rattata now!"        
      }
      if (gameData.rat >= 1) {
        document.getElementById('rat').style.display = 'inline';
        document.getElementById('oaktext').innerHTML = "Good job! There are many Pokémon for you to catch, so try to catch 'em all! You can also use boosters to get pokecoins faster!"        
      }
    }
    </script>
  </body>
</html>
