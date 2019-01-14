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