# Pig-dice-game
#### by **UWABIKIRAMARIYA Roselyne**
## Description
This pig-dice-game website require two players where the first players rolls a dice, and mark scores and he holds the scores but if the rolling turns to one, it will be the second player's turn vice-versa. A 11th January 2019.
**Codes**
```
var rolling = function() {
  return Math.floor(Math.random() * 6) + 1;
}

function Player(roll, tempscore, totalscore, playername) {
  this.roll = 0;
  this.tempscore = 0;
  this.totalscore = 0;
  this.playername;
}
Player.prototype.onedie = function() {
  if (this.roll == 1) {
    this.tempscore = 0;
    alert("1 is not in your favour " + this.playername + ", your turn is over!");
  } else {
    this.tempscore += this.roll;
  }
}
Player.prototype.hold = function() {
  this.totalscore += this.tempscore;
  this.tempscore = 0;
  alert(this.playername + ", your held your score, your turn is over.");
}
Player.prototype.proGamer = function() {
  if (this.totalscore == 100) {
    alert(this.playername + ", you are Master Dicer!!");
  }
}
Player.prototype.newGame = function() {
  this.roll = 0;
  this.tempscore = 0;
  this.totalscore = 0;
  this.playername = ('');
}
```
## Setup/Installation Requirements
* Ubuntu oparating system
* Visual studio code
* Github
* Google chrome to display webpages
* Bootstrap 

These above, are the tools that i use to acheive my desires during this class, at WeCode moringa school
## BDD
Two playes enter their names, one player starts to play by clicking **Roll**,to roll the dice, each roll comes up with its score, and the summation is holded by the player where he/she clicks **Hold**. if any player rolls a **1** it scores a **0** and it is the other player's turn, vice-versa.

The winner is announced when the total csore of one play is greater or equal too 100. and then after they start a new game or reset the current one. 
## Technologies Used
1. HTML5
2. CSS
3. README
4. Javascript
5. jQuery
## Support and contact details
I appreciate everyone's support through comment or connection.
if you want to do so, reach me at 
* email: *mariadelarosita078@gmail.com*
* phone cell **+250786421009**

My encouragment , my motivation is from my own instict, my parents,my team mentor, my support from WeCode Moringa school.
## Links
If you want to check out my work just click *https://roxaline.github.io/Pig-dice-game/*
### License
*This is my own work.*

MIT Copyright (c) 2019