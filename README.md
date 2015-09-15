# composicion-con-for
//variables 

float  lu = 0;
float fin = 0;
int gif = 1;
PFont letra;
float  chin=3.1;
float antes = 5.1;
float zeta = 1 ;

//una vez

void setup (){
  size(1000,1000);
 letra = loadFont("atriskyouth-100.vlw");
}


void draw(){
  background(#131440);
  text("MONO",490,650);
  
   lu=lu+(chin*gif);
  fin=fin+(antes*zeta);
  
  
  
  
    if (lu > 1000||lu < 0){
    gif= gif *-1;
  }
    if (fin > 1000 || fin < 0){
    zeta = zeta *-1;
  }
  
     if (fin > 200 || fin < 100){
   fill(#4D9848);
  }else{
    fill(#7E9848);
  }
   if (fin > 400|| fin < 200){
   fill(#4D50E0);
  }else{
    fill(#7E9848);
  }
   if (fin > 600|| fin < 400){
   fill(#4D50E0);
  }else{
    fill(255);
  }

  ellipse(fin,lu,30,30);
  
  //esferas
 for( int a=30; a < 1000; a= a +80){
  for( int b = 10 ; b < 1000; b= b+100)
  ellipse(a,b,30,30);
   }
     

     
     for( int c=10; c < 1000; c= c +100){
    for( int d = 10 ; d< 1000; d= d+100)
 
    ellipse(c,d,40,40);
     ellipse(fin,lu,30,30);
     
 }
   }

