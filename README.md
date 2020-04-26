# Processing-code-example


펜 만들기 
<pre>
<code>
void setup(){
  size(500,500);
  stroke(0,0,255);
  strokeWeight(16);
}
void draw(){
  if(mousePressed){
    line(pmouseX, pmouseY, mouseX, mouseY);
  }
}
</code>
</pre>

원을 좌우로 이동

<pre>
<code>
void setup(){

  size(500,500);

 

}

int i;

void draw(){  

  background(0);

  fill(0,0,255);

  ellipse(i++,250, 100, 100);

  if(i>500) i = 0;

 

}
</code>
</pre>

배너 만들기 
<pre>
<code>
void setup(){
  size(800,400);
  textSize(128);
}
int i, a =1;
void draw(){
  background(194);
  if(keyPressed)
    a = key -'0';
  text("Graphics", i = i+a, 200);
  fill(255,0,0);
  if(i>800 || i <0)
    i =0;
}
</code>
</pre>

공의 회전 및 크기 조정 

<pre>
<code>
void setup(){
  size(500,500);
  rectMode(CENTER);
}
float f;
void draw(){
  translate(mouseX, mouseY);
  rotate(f);
  scale(sin(f)+1);
  f = f+0.05;
  fill(0,255,0);
  rect(0, 0, 80,80);
  fill(255,0,255);
  ellipse(0, 0, 80,80);
}
</code>
</pre>

PShape 예제 변형 

<pre>
<code>

void setup(){
  size(400,400);
}
float f;
void draw() {
  background(0,255,0);
  translate(mouseX, mouseY);
  scale(sin(f)+1);
  f = f+0.05;
  fill(255,0,0);
  stroke(255,0,0);
  strokeWeight(5);
  beginShape();
  vertex(0, -50);
  vertex(14, -20);
  vertex(47, -15);
  vertex(23, 7);
  vertex(29, 40);
  vertex(0, 25);
  vertex(-29, 40);
  vertex(-23, 7);
  vertex(-47, -15);
  vertex(-14, -20);
  endShape(CLOSE);
}
</code>
</pre>
