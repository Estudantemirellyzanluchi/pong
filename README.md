//variveldabolinha
let xBolinha = 650;
let yBolinha = 200;
let diâmetro = 20;
let raio = diâmetro / 2;

//velocidade da bolinha
let velocidadexBolinha = 4;
let velocidadeyBolinha = 4;
let raqueteComprimento = 7;
let raqueteAltura = 70;

//variáveis da raquete 
let xRaquete = 3;
let yRaquete = 150;

//variáveis do oponente 
let xRaqueteOponente = 1290;
let yRaqueteOponente = 150;
let velocidadeYOponente;

let colidiu = false;

//placar do jogo
let meusPontos = 0;
let pontosDoOponente = 0;

//sons do jogo
let raquetada;
let ponto;
let trilha;

function preload(){
 trilha = loadSound("trilha.mp3");
 ponto = loadSound("ponto.mp3");
 raquetada = loadSound("raquetada.mp3");
 }
 
function setup() {
 createCanvas(1300, 400);
 trilha.loop();
 }
 
function draw() {
    background(0);
    mostraBolinha();
    
