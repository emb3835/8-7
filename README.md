# 8-7
void setup() {size(480, 120);smooth();}void draw() {background(204);owl(110, 110);owl(180, 110);background(204);for (int x = 35; x < width + 70; x += 70) {
owl(x, 110);}}void owl(int x, int y) {pushMatrix();translate(x, y);stroke(0);strokeWeight(70);line(0, -35, 0, -65); // BodynoStroke();fill(255-x);ellipse(-17.5, -65, 35, 35); // Left eye domeellipse(17.5, -65, 35, 35); // Right eye domearc(0, -65, 70, 70, 0, PI); // Chinfill(0);ellipse(-14, -65, 8, 8); // Left eyeellipse(14, -65, 8, 8); // Right eyequad(0, -58, 4, -51, 0, -44, -4, -51); // BeakpopMatrix();}
