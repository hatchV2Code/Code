var seconds = 0;
var x = 0;
var img;
//robot
var xPos = 0;
var yPos = 100;
var xSpeed = 5;

//second robot
var xPos2 = 0;
var yPos2 = 100;

function setup() {
  createCanvas(400, 400);
  textAlign(CENTER, CENTER);
  let milliseconds = millis();
  img = createImg("https://climatekids.nasa.gov/review/air-pollution/air-polution-illustration.png", "hi");
  img.hide();
}

function timer() {
  milliseconds = millis();
  seconds = floor(milliseconds / 1000);
}

function robot() {
  stroke(0);
  strokeWeight(1);
  //body
  fill(100, 100, 100);
  rect(200, 220, 50, 80, 10);
  //head
  fill(155, 155, 155);
  rect(200, 200, 50, 30, 50);
  rect(200, 200, 50, 20, 10);

  //filter
  fill(155, 155, 155);
  ellipse(225, 200, 40, 5);

  //eyes
  rect(205, 205, 15, 15);
  rect(230, 205, 15, 15);
  //pupil
  fill(0);
  rect(210, 210, 5, 5);
  fill(0);
  rect(235, 210, 5, 5);
}

function draw() {
  background(255);
  image(img, 0, 0, img.elt.width, img.elt.height);
  timer();

  //light
  noStroke();
  fill(255, 255, 255, 100);
  rect(0, 0, 400, 400);

  fill(255);
  noStroke();
  //text(seconds + "\n" + milliseconds, 10, 200);

  if (milliseconds > 400 && milliseconds < 5000) {
    fill(0);
    stroke(0);
    textSize(30);
    text("Air pollution is a problem", 200, 220);
  }

  if (milliseconds > 2000 && milliseconds < 5000) {
    fill(0);
    stroke(0);
    textSize(30);
    text("But I have a solution!", 200, 260);
  }

  if (seconds >= 5 && seconds < 8) {
    fill(0);
    stroke(0);
    textSize(30);
    text("Introducing", 200, 250);
  }

  if (seconds >= 8 && seconds <= 10) {

    //animate
    xPos += xSpeed;
    translate(xPos - 300, yPos);
    robot();
    resetMatrix(); //resets position, to not affect position of code below
    //robot stops
    if (xPos > 340) {
      xPos = 340;
      noStroke();
      fill(0);
      textSize(30);
      text("Elecktro.v1", 170, 250);
    }
    resetMatrix();
  }

  if (seconds >= 10.5 && seconds <= 15) {
    //duplicate robot (without movement)
    translate(xPos2 + 45, yPos2);

    robot();

    resetMatrix();

    stroke(0);
    fill(0);
    textSize(30);
    text("My solution is a filter that has \n a circuit inside it which detects\n where there is air pollution", 195, 130);
  }

  if (seconds >= 15.5 && seconds <= 20) {
    translate(xPos2 + 45, yPos2);
    robot();
   
    resetMatrix(); //resets the positions from previous translate
   
    stroke(0);
    fill(0);
    textSize(30);
    text("It will suck all the air pollution \n inside its body, then it will \n decompose and turn into \n clean air", 195, 130);
  }

  if (seconds >= 20.5 && seconds <= 25) {
    translate(xPos2 + 45, yPos2);
    robot();
   
    resetMatrix(); //resets the positions from previous translate
   
    stroke(0);
    fill(0);
    textSize(30);
    text("Watch this robot decompose \n the pollution inside its body \n to produce clean air", 195, 130);
  }

  if (seconds >= 25.5 && seconds <= 26) {
    //animate
    xPos -= xSpeed;
    translate(xPos - 300, yPos);
    robot();
    //movement
    if (xPos < 200) {
      xPos = 200;
    }
    resetMatrix();
  }

  if (seconds >= 26.5 && seconds <= 29) {
    //robot (without movement)
    translate(xPos2 - 105, yPos2);
    robot();
    fill(50, 50, 50);
    rect(210, 195, 30, 5);
    fill(155, 155, 155);
    ellipse(225, 195, 40, 5);

    resetMatrix();
   
    stroke(0);
    fill(0);
    textSize(30);
    text("SWOOSH", 195, 130);
  }

  if (seconds >= 29.5 && seconds <= 38) {
    translate(xPos2 - 105, yPos2);
    robot();
    fill(50, 50, 50);
    rect(210, 195, 30, 5);
    fill(155, 155, 155);
    ellipse(225, 195, 40, 5);

    resetMatrix();

    noStroke();
    fill(209, 224, 227);
    rect(0, 0, 400, 180, 50);
    fill(209, 224, 227);
    rect(200, 20, 400, 180, 50);
    fill(209, 224, 227);
    rect(150, 110, 70, 180, 50);
    fill(209, 224, 227);
    rect(0, 110, 30, 258);

    stroke(0);
    fill(0);
    textSize(30);
    text("Voila, clean air!", 195, 130);
  }

}
