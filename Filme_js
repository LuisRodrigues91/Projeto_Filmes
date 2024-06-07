let campoIdade
let campoFantasia
let campoAventura


function setup() {
  createCanvas(800, 400);
  createElement("h2","Recomendador de filmes")
  createSpan ("Sua Idade")
  campoIdade = createInput ("5")
  campoFantasia = createCheckbox ("Gosta de  Fantasia?")
  campoAventura = createCheckbox ("Gosta de Aventura?")
}

function draw() {
  background("white");
  let idade = campoIdade.value();
  let gostaDeFantasia = campoFantasia.checked();
  let gostaDeAventura = campoAventura.checked();
  let recomendacao = geraRecomendacao (idade,gostaDeFantasia, gostaDeAventura);
  
  fill (color(76,0,115));
  textAlign (CENTER,CENTER);
  textSize(38);
  text(recomendacao,width/2,height/2);
  }

function geraRecomendacao (idade,gostaDeFantasia,gostaDeAventura){
  if(idade >=10){
    if(idade >=14){
      return "O Menino que descubriu o Vento";
    } else {
      if (idade >=12){
        if(gostaDeFantasia||gostaDeAventura){
          return "Homem Aranha: no aranhaverso";
        } else{
          return "Ladrões de Bicicleta";
        } 
      } else {
        if (gostaDeFantasia) {
          return "As Aventura de Pi";
        } else {
          return "Depois da Chuva";
        }
      }
    }
  } else {
    if(gostaDeFantasia){
      return "A Viagem de Chihiro";
    } else{
      return "O feitiço do Tempo"
    }
  }
}





