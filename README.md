
<a href="http://public.district196.org/rhs/"><img src="http://public.district196.org/rhs/imagesmain/crest150_trans.png" title="Rosemount High School" alt="RHS"></a>





# Senior-Year-Protfolio

> This portfolio will showcase the projects that I have been working on in my senior year of High School.


# Java Portfolio


<details>
<summary>WebPage</summary> 
<br>(https://kantab.github.io/testWeb/)
This project was desgined to give an introduction to HTML and JS. This was the first web page I made. 
The hardest part was understanding a new launage.
 </br>
</details>
<details>
<summary>Lightning</summary>
<br>(https://kantab.github.io/lightning2/)
This project was desgined to practice using Math.random. The hardest part for the project was figuring out the layout of where the lighting starts and ends.
 </br>
</details>
<details>
<summary>Dice</summary>
<br>(https://kantab.github.io/dice3/)
The project goal was to display dice on the screen and out put their sum. This was my favorite project beacuse I was able to put my own creative spin on it. I displayed the dice as a game where you would win if your sum of 3 dice was 3, or if all 3 numbers were the same.
 </br>
</details>
<details>
<summary>Chemotaxis JS</summary>
<br>( https://kantab.github.io/chemotaxis4/)
The project was desgined to learn a bit more with arrylist. The hardest part of this project was once I was complete I converted the code into JavaScript. This was the first time I had worked with JavaScript. 
 </br>
</details>
<details>
<summary>Starfeilds</summary>
<br>
 ```java
 Particle [] p = new Particle[100];
Particle [] p2 = new Particle[100];
Particle [] p3 = new Particle[100];
void setup(){
size(800,600);
for(int i =0; i<p.length; i++){
 p[i]= new NormalParticle();
 p2[i]= new oddBallParticle();
 p3[i]= new jumpoParticle();
}
for(int j =0; j<p2.length; j++){
//p2[j]= new oddBallParticle();
}
  
}
void draw(){
  
  
  noStroke();
  fill( 2, 0, 0, 5);
  rect(0, 0, width, height,50);
  for(int i=0; i<p.length; i++){
    p[i].move();
    p[i].show();
    p2[i].move();
    p2[i].show();
    p3[i].move();
    p3[i].show();
  }
}

interface Particle{
  void show();
  void move();
  
}
////////////////////////////////////////////////////////
class NormalParticle implements Particle {
  double x, y, speed, angle;

  public NormalParticle() {
    x=width/2-100;
    y=height/2-100;
    speed=5;
    angle=0.25;
  }
  void move() {
    /* if(angle>0.025){
     angle-=0.05;
     }
     else {
     angle+=0.05;
     }
     */
    if (angle>0) {
      angle+=0.05;
    }
    x+=Math.cos(angle)*speed;
    y+=Math.sin(angle)*speed;
    angle+=0.025;
  }
  void show() {
    fill(0, 255, 200);
    //fill((int)((Math.random()*200)+150), (int)((Math.random()*200)+150), (int)((Math.random()*200)+150));
    ellipse((int)x, (int)y, 20, 20);
  }
}
//////////////////////////////////////////////////////////
class jumpoParticle implements Particle {
  double x, y, speed, angle;

  public jumpoParticle() {
    x=width/2+100;
    y=height/2-100;
    speed=5;
    angle=0.25;
  }
  void move() {
    x+=Math.cos(angle)*speed;
    y+=Math.sin(angle)*speed;
    angle+=0.025;
    
  }
  void show() {
    fill((int)((Math.random()*200)+150), (int)((Math.random()*200)+150), (int)((Math.random()*200)+150));
    ellipse((int)x, (int)y, 80, 30);
    
    ellipse((int)x, (int)y-10, 40, 40);
  }
}
/////////////////////////////////////////////
class oddBallParticle implements Particle {
  double x, y, speed, angle;

  public oddBallParticle() {
    x=width/2;
    y=height/2;
    speed=Math.random()*5;
    angle=Math.random()*Math.PI*8;
  }
  void move() {
    x+=Math.cos(angle)*speed;
    y+=Math.sin(angle)*speed;
    angle+=0.025;
    if (x>500) {
      x=100;
      speed*=-1;
    }
    if (y>500) {
      y=300;
      
      speed*=-1;
    }
  }
  void show() {
    fill((int)((Math.random()*200)+150), (int)((Math.random()*200)+150), (int)((Math.random()*200)+150));
    ellipse((int)x, (int)y, 20, 20);
  }
}
//////////////////////////////////////////////////
 
 ```
This project was by far the hardest for me to understand. I had a hard time understaning how th objects were to be displayed on the screen and the angle in which they moved. I had to partner up with other class mates so they could show me how it worked.
 </br>
</details>

***

 This is my most worthy peice of code so far. This code is from my JS chemotaxis. I like this code because it was not only a little tricky to figure out how to cycle through the images but I then had to take this code and change it from Java to JavaScript, a launage I was learning at the time. What was tricky about cycling through was the fact when I had a mousePressed method, when I would increase the counter that would in turn change the pictures it would add more then once when the mouse was clicked/ pressed. How i solved this is i created a boolean that would flip if the mouse was pressed and when it wasnt it would be fliped back. This then made it able to only increase by one when the mouse was pressed. 
```Java
 if (!mousePressed) {
    this.ss = true;
  }
  if(mousePressed){
    this.ss=false;
  }
  
    
    if(this.clic==0){
    image(this.img1, this.x, this.y);
    }
    if(this.clic==1){
    image(this.img2, this.x, this.y);
    
    }
    if(this.clic==2){
    image(this.img4, this.x, this.y);
    
    }
    if(this.clic>2){
    this.clic=0;
    
    }
    

```
# C++ Portfolio

<details>
<summary>Payroll</summary> 
<br>(https://kantab.github.io/testWeb/)
This project was one that I worked on in my introduction to C++ class I took at Inver Hills Community College. This project was desgined to teach us how to use things such as setprecision, switchs, try/ catch statements, interfaces, user inputs, and a lot of the key foundations to help learn and understand C++. We made a few difernt variations of this project and this is the final one.
 </br>
</details>


