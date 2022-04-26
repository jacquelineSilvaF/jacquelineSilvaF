# Oii👋

Meu nome é Jacqueline e sou estudante do curso de Design na UFPE.
Tenho interesse na área de Web Design/Font-end.

- ✨Consigo utilizar **HTML** e **CSS**.
- 📝Atualmente estou aprendendo **P5.Js**/**Processing**.
- 📚Pretendo me aprofundar mais em **JavaScript**.

🔗Links:
<div>

  <a href="mailto:silvafonseca.jacqueline@gmail.com" target="_blank"> <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"> </a>
  <a href="https://www.linkedin.com/in/jacquelinesilvafonseca/" target="_blank"> <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"> </a>

</div>

```
//Declarar um conjunto de variáveis para utilizar nas funções//
let ball = {
  x: 200,
  y: 100, 
  xSpeed: 5,
  ySpeed: 5
}


let r, g, b;

//Função que muda a cor da bola
function ballcolor() {
  r = random(100, 256);
  g = random(100, 256);
  b = random(100, 256);
}


function setup() {
  createCanvas(700, 500);
  ballcolor();
}

function draw() {
  
  background(0);
  
  ballImage();
  move();
  bounce();
   
}

//Função que faz o movimento diagonal da bola
function move() {
  
  ball.x = ball.x + ball.xSpeed;
  ball.y = ball.y + ball.ySpeed;
  
}

//Função que faz a bola voltar quando bate o limite do canvas
function bounce () {
  if (ball.x + 45 == width || ball.x == 45) {
    
    ball.xSpeed = ball.xSpeed * -1;
    
    ballcolor();
    
  }
  
  if (ball.y + 45 == height || ball.y == 45) {
    
    ball.ySpeed = ball.ySpeed * -1;
    
    ballcolor();
    
  }
}

//Função que desenha a bola
function ballImage() {
  
  fill(r, g, b);
  noStroke();
  ellipse(ball.x, ball.y, 90);
  
}

```
