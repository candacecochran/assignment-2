# assignment-two
assignment 2

var mr_dragon; //this is global variable

function preload() {
  pineapple = loadImage("./pine.png");
  cool = loadImage("./cool.png");


}

function setup() {
  createCanvas(700,700);
  background(187, 143, 206); //this is a color in RGBA colorspace : red, green, blue and alpha (opacity)

  for(var counter=0;counter<6;counter=counter+1){
    push();
    translate(0+counter*100,0);
    rotate(radians(0));
      image(pineapple,0,0,300,300);
      image(cool,0,0,0*counter,0*counter );

    pop();

  }

}
