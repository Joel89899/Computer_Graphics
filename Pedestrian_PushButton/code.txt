#include <GL/glut.h>
#include <GL/GL.h>
#include <GL/GLU.h>
#include <math.h>
bool check = true;
float g;


void display(void)
{
	glClear(GL_COLOR_BUFFER_BIT);
	//Black Road
	glBegin(GL_POLYGON);
	glColor3f(0, 0, 0);
	glVertex3f(200, 200, 0);
	glVertex3f(0, 40, 0);
	glVertex3f(0, 0, 0);
	glVertex3f(500, 0, 0);
	glVertex3f(500, 40, 0);
	glVertex3f(300, 200, 0);
	glEnd();

	//Black Road- 2
	glBegin(GL_POLYGON);
	glColor3f(0, 0, 0);
	glVertex3f(220, 235, 0);
	glVertex3f(200, 200, 0);
	glVertex3f(300, 200, 0);
	glVertex3f(275, 235, 0);
	glEnd();


	//Black Road- 4
	glBegin(GL_POLYGON);
	glColor3f(0, 0, 0);
	glVertex3f(220, 235, 0);
	glVertex3f(200, 200, 0);
	glVertex3f(100, 200, 0);
	glVertex3f(100, 235, 0);
	glEnd();

	//Black Road- 5
	glBegin(GL_POLYGON);
	glColor3f(0, 0, 0);
	glVertex3f(275, 235, 0);
	glVertex3f(300, 200, 0);
	glVertex3f(340, 200, 0);
	glVertex3f(340, 255, 0);
	glEnd();

	//White lines
	glBegin(GL_POLYGON);
	glColor3f(1, 1, 1);
	glVertex3f(204, 200, 0);
	glVertex3f(200, 200, 0);
	glVertex3f(0, 40, 0);
	glVertex3f(0, 30, 0);
	glEnd();
	glBegin(GL_POLYGON);
	glVertex3f(300, 200, 0);
	glVertex3f(296, 200, 0);
	glVertex3f(500, 30, 0);
	glVertex3f(500, 40, 0);
	glEnd();

	//Left Side Red lines
	glBegin(GL_POLYGON);
	glColor3f(1, 0, 0);
	glVertex3f(200, 204, 0);
	glVertex3f(0, 50, 0);;
	glVertex3f(0, 40, 0);
	glVertex3f(200, 200, 0);
	glEnd();

	//White Bars
	glBegin(GL_QUADS);
	glColor3f(1, 1, 1);
	glVertex3f(245, 0, 0);
	glVertex3f(245, 40, 0);
	glVertex3f(255, 40, 0);
	glVertex3f(255, 0, 0);
	glVertex3f(246, 60, 0);
	glVertex3f(246, 100, 0);
	glVertex3f(254, 100, 0);
	glVertex3f(254, 60, 0);
	glVertex3f(247, 120, 0);
	glVertex3f(247, 160, 0);
	glVertex3f(253, 160, 0);
	glVertex3f(253, 120, 0);
	glVertex3f(248, 180, 0);
	glVertex3f(248, 200, 0);
	glVertex3f(252, 200, 0);
	glVertex3f(252, 180, 0);
	glVertex3f(256, 180, 0);
	glVertex3f(256, 200, 0);
	glVertex3f(260, 200, 0);
	glVertex3f(260, 180, 0);
	glVertex3f(264, 180, 0);
	glVertex3f(264, 200, 0);
	glVertex3f(268, 200, 0);
	glVertex3f(268, 180, 0);
	glVertex3f(272, 180, 0);
	glVertex3f(272, 200, 0);
	glVertex3f(276, 200, 0);
	glVertex3f(276, 180, 0);
	glVertex3f(280, 180, 0);
	glVertex3f(280, 200, 0);
	glVertex3f(284, 200, 0);
	glVertex3f(284, 180, 0);
	glVertex3f(288, 180, 0);
	glVertex3f(288, 200, 0);
	glVertex3f(292, 200, 0);
	glVertex3f(292, 180, 0);
	glVertex3f(240, 180, 0);
	glVertex3f(240, 200, 0);
	glVertex3f(244, 200, 0);
	glVertex3f(244, 180, 0);
	glVertex3f(232, 180, 0);
	glVertex3f(232, 200, 0);
	glVertex3f(236, 200, 0);
	glVertex3f(236, 180, 0);
	glVertex3f(224, 180, 0);
	glVertex3f(224, 200, 0);
	glVertex3f(228, 200, 0);
	glVertex3f(228, 180, 0);
	glVertex3f(216, 180, 0);
	glVertex3f(216, 200, 0);
	glVertex3f(220, 200, 0);
	glVertex3f(220, 180, 0);
	glVertex3f(208, 180, 0);
	glVertex3f(208, 200, 0);
	glVertex3f(212, 200, 0);
	glVertex3f(212, 180, 0);
	// Left side Whites
	glVertex3f(180, 214, 0);
	glVertex3f(180, 210, 0);
	glVertex3f(135, 210, 0);
	glVertex3f(135, 214, 0);
	glVertex3f(180, 221, 0);
	glVertex3f(180, 217, 0);
	glVertex3f(135, 217, 0);
	glVertex3f(135, 221, 0);
	glVertex3f(180, 228, 0);
	glVertex3f(180, 224, 0);
	glVertex3f(135, 224, 0);
	glVertex3f(135, 228, 0);
	glEnd();

	//Right side red line
	glBegin(GL_POLYGON);
	glColor3f(1, 0, 0);
	glVertex3f(300, 204, 0);
	glVertex3f(300, 200, 0);;
	glVertex3f(400, 120, 0);
	glVertex3f(400, 125, 0);
	glEnd();

	//Right Side Walk
	glBegin(GL_POLYGON);
	glColor3f(0.827451, 0.827451, 0.827451);
	glVertex3f(300, 204, 0);
	glVertex3f(400, 125, 0);;
	glVertex3f(400, 165, 0);
	glVertex3f(340, 204, 0);
	glEnd();

	//right building
	glBegin(GL_POLYGON);
	glColor3f(0.56, 0.31, 0.13);
	glVertex3f(340, 204, 0);
	glVertex3f(340, 310, 0);
	glVertex3f(400, 340, 0);
	glVertex3f(400, 165, 0);
	glEnd();

	//Left Side walk
	glBegin(GL_POLYGON);
	glColor3f(0.827451, 0.827451, 0.827451);
	glVertex3f(125, 204, 0);
	glVertex3f(0, 125, 0);;
	glVertex3f(0, 50, 0);
	glVertex3f(200, 204, 0);
	glEnd();

	//Front Side walk - L
	glBegin(GL_POLYGON);
	glColor3f(0.827451, 0.827451, 0.827451);
	glVertex3f(100, 235, 0);
	glVertex3f(220, 235, 0);;
	glVertex3f(240, 255, 0);
	glVertex3f(100, 255, 0);
	glEnd();

	//Front Side walk - R
	glBegin(GL_POLYGON);
	glColor3f(0.827451, 0.827451, 0.827451);
	glVertex3f(275, 235, 0);
	glVertex3f(340, 235, 0);;
	glVertex3f(340, 255, 0);
	glVertex3f(260, 255, 0);
	glEnd();

	//Front Side walk - Mid
	glBegin(GL_POLYGON);
	glColor3f(0.827451, 0.827451, 0.827451);
	glVertex3f(220, 235, 0);
	glVertex3f(275, 235, 0);
	glVertex3f(260, 255, 0);
	glVertex3f(240, 255, 0);
	glEnd();

	//Left Building
	glBegin(GL_POLYGON);
	glColor3f(0.698039, 0.133333, 0.133333);
	glVertex3f(100, 295, 0);
	glVertex3f(0, 300, 0);;
	glVertex3f(0, 125, 0);
	glVertex3f(100, 188, 0);
	glEnd();

	//Tree1
	glBegin(GL_POLYGON);
	glColor3f(0.486275, 0.988235, 0);
	glVertex3f(115, 235, 0);
	glVertex3f(100, 235, 0);
	glVertex3f(90, 225, 0);
	glVertex3f(90, 215, 0);
	glVertex3f(100, 205, 0);
	glVertex3f(115, 205, 0);
	glVertex3f(125, 215, 0);
	glVertex3f(125, 225, 0);
	glEnd();
	//Stem1
	glBegin(GL_POLYGON);
	glColor3f(0.870588, 0.721569, 0.529412);
	glVertex3f(103.5, 190, 0);
	glVertex3f(100, 170, 0);
	glVertex3f(115, 170, 0);
	glVertex3f(112.5, 190, 0);
	glVertex3f(115, 205, 0);
	glVertex3f(100, 205, 0);
	glEnd();

	//Tree2
	glBegin(GL_POLYGON);
	glColor3f(0.486275, 0.988235, 0);
	glVertex3f(84, 258, 0);
	glVertex3f(66, 258, 0);
	glVertex3f(54, 246, 0);
	glVertex3f(54, 234, 0);
	glVertex3f(66, 222, 0);
	glVertex3f(84, 222, 0);
	glVertex3f(96, 234, 0);
	glVertex3f(96, 246, 0);
	glEnd();
	//Stem2
	glBegin(GL_POLYGON);
	glColor3f(0.870588, 0.721569, 0.529412);
	glVertex3f(69, 204, 0);
	glVertex3f(66, 150, 0);
	glVertex3f(84, 150, 0);
	glVertex3f(81, 202.8, 0);
	glVertex3f(84, 222, 0);
	glVertex3f(66, 222, 0);
	glEnd();

	//Tree3
	glBegin(GL_POLYGON);
	glColor3f(0.486275, 0.988235, 0);
	glVertex3f(40, 175, 0);
	glVertex3f(25, 175, 0);
	glVertex3f(15, 165, 0);
	glVertex3f(15, 155, 0);
	glVertex3f(25, 145, 0);
	glVertex3f(40, 145, 0);
	glVertex3f(50, 155, 0);
	glVertex3f(50, 165, 0);
	glEnd();
	//Stem3
	glBegin(GL_POLYGON);
	glColor3f(0.870588, 0.721569, 0.529412);
	glVertex3f(27.5, 130, 0);
	glVertex3f(25, 110, 0);
	glVertex3f(40, 110, 0);
	glVertex3f(37.5, 129, 0);
	glVertex3f(40, 145, 0);
	glVertex3f(25, 145, 0);
	glEnd();

	//Pole
	glBegin(GL_POLYGON);
	glColor3f(0.439216, 0.541176, 0.564706);
	glVertex3f(180, 240, 0);
	glVertex3f(180, 275, 0);
	glVertex3f(200, 275, 0);
	glVertex3f(200, 240, 0);
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(0.439216, 0.541176, 0.564706);
	glVertex3f(187.5, 204, 0);
	glVertex3f(187.5, 240, 0);
	glVertex3f(192.5, 240, 0);
	glVertex3f(192.5, 204, 0);
	glEnd();

	//ligths RED
	glBegin(GL_POLYGON);
	glColor3f(1, 0, 0);
	glVertex3f(185, 270, 0);
	glVertex3f(185, 265, 0);
	glVertex3f(195, 265, 0);
	glVertex3f(195, 270, 0);
	glEnd();

	//Lights YELLOW
	glBegin(GL_POLYGON);
	glColor3f(1.00, 0.98, 0.83);
	glVertex3f(185, 260, 0);
	glVertex3f(185, 255, 0);
	glVertex3f(195, 255, 0);
	glVertex3f(195, 260, 0);
	glEnd();
	//Lights GREEN
	glBegin(GL_POLYGON);
	glColor3f(0.85, 1.00, 0.86);
	glVertex3f(185, 250, 0);
	glVertex3f(185, 245, 0);
	glVertex3f(195, 245, 0);
	glVertex3f(195, 250, 0);
	glEnd();

	//On the Right Side of The Road

	//Pole
	glBegin(GL_POLYGON);
	glColor3f(0.439216, 0.541176, 0.564706);
	glVertex3f(307.5, 240, 0);
	glVertex3f(307.5, 275, 0);
	glVertex3f(327.5, 275, 0);
	glVertex3f(327.5, 240, 0);
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(0.439216, 0.541176, 0.564706);
	glVertex3f(315, 204, 0);
	glVertex3f(315, 240, 0);
	glVertex3f(320, 240, 0);
	glVertex3f(320, 204, 0);
	glEnd();

	//ligths RED
	glBegin(GL_POLYGON);
	glColor3f(1, 0, 0);
	glVertex3f(312.5, 270, 0);
	glVertex3f(312.5, 265, 0);
	glVertex3f(322.5, 265, 0);
	glVertex3f(322.5, 270, 0);
	glEnd();

	//Lights YELLOW
	glBegin(GL_POLYGON);
	glColor3f(1.00, 0.98, 0.83);
	glVertex3f(312.5, 260, 0);
	glVertex3f(312.5, 255, 0);
	glVertex3f(322.5, 255, 0);
	glVertex3f(322.5, 260, 0);
	glEnd();
	//Lights GREEN
	glBegin(GL_POLYGON);
	glColor3f(0.85, 1.00, 0.86);
	glVertex3f(312.5, 250, 0);
	glVertex3f(312.5, 245, 0);
	glVertex3f(322.5, 245, 0);
	glVertex3f(322.5, 250, 0);
	glEnd();

	//Human Body
	glBegin(GL_LINE_STRIP);
	glColor3f(0.28, 0.23, 0.13);
	glVertex3f(165, 235, 0);
	glVertex3f(165, 220, 0);
	glVertex3f(160, 204, 0);
	glEnd();
	glBegin(GL_LINE_STRIP);
	glColor3f(0.28, 0.23, 0.13);
	glVertex3f(155, 230, 0);
	glVertex3f(165, 225, 0);
	glVertex3f(175, 230, 0);
	glEnd();
	glBegin(GL_LINES);
	glVertex3f(165, 220, 0);
	glVertex3f(170, 204, 0);
	glEnd();
	//Human Head
	float theta;
	glBegin(GL_POLYGON);
	glColor3f(0.28, 0.23, 0.13);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(165 + 5 * cos(theta), 240 + 5 * sin(theta));
	}
	glEnd();

	//CLOUDS 1
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(50 + 15 * cos(theta), 400 + 10 * sin(theta));
	}
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(60 + 15 * cos(theta), 410 + 10 * sin(theta));
	}
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(70 + 15 * cos(theta), 400 + 10 * sin(theta));
	}
	glEnd();


	//CLOUDS 2
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(150 + 15 * cos(theta), 425 + 10 * sin(theta));
	}
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(160 + 15 * cos(theta), 435 + 10 * sin(theta));
	}
	glEnd();
	glBegin(GL_POLYGON);
	glColor3f(1.0, 1.0, 1.0);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(170 + 15 * cos(theta), 425 + 10 * sin(theta));
	}
	glEnd();

	//SUN
	glBegin(GL_POLYGON);
	glColor3f(0.992, 0.721, 0.074);
	for (int i = 0; i < 360; i++)
	{
		theta = i * 3.142 / 180;
		glVertex2f(350 + 20 * cos(theta), 450 + 20 * sin(theta));
	}
	glEnd();


	glFlush();



}

void keyDown(unsigned char key, int x, int y)
{
	switch (key)
	{
	case 'g': {
		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(0.71, 0.40, 0.44);
		glVertex3f(185, 270, 0);
		glVertex3f(185, 265, 0);
		glVertex3f(195, 265, 0);
		glVertex3f(195, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1.00, 0.98, 0.83);
		glVertex3f(185, 260, 0);
		glVertex3f(185, 255, 0);
		glVertex3f(195, 255, 0);
		glVertex3f(195, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0, 1.00, 0);
		glVertex3f(185, 250, 0);
		glVertex3f(185, 245, 0);
		glVertex3f(195, 245, 0);
		glVertex3f(195, 250, 0);
		glEnd();

		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(0.71, 0.40, 0.44);
		glVertex3f(312.5, 270, 0);
		glVertex3f(312.5, 265, 0);
		glVertex3f(322.5, 265, 0);
		glVertex3f(322.5, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1.00, 0.98, 0.83);
		glVertex3f(312.5, 260, 0);
		glVertex3f(312.5, 255, 0);
		glVertex3f(322.5, 255, 0);
		glVertex3f(322.5, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0, 1.00, 0);
		glVertex3f(312.5, 250, 0);
		glVertex3f(312.5, 245, 0);
		glVertex3f(322.5, 245, 0);
		glVertex3f(322.5, 250, 0);
		glEnd();
		glFlush();

	}
			break;
	case 'y': {
		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(0.71, 0.40, 0.44);
		glVertex3f(185, 270, 0);
		glVertex3f(185, 265, 0);
		glVertex3f(195, 265, 0);
		glVertex3f(195, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1, 1, 0);
		glVertex3f(185, 260, 0);
		glVertex3f(185, 255, 0);
		glVertex3f(195, 255, 0);
		glVertex3f(195, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0.85, 1.00, 0.86);
		glVertex3f(185, 250, 0);
		glVertex3f(185, 245, 0);
		glVertex3f(195, 245, 0);
		glVertex3f(195, 250, 0);
		glEnd();

		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(0.71, 0.40, 0.44);
		glVertex3f(312.5, 270, 0);
		glVertex3f(312.5, 265, 0);
		glVertex3f(322.5, 265, 0);
		glVertex3f(322.5, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1, 1, 0);
		glVertex3f(312.5, 260, 0);
		glVertex3f(312.5, 255, 0);
		glVertex3f(322.5, 255, 0);
		glVertex3f(322.5, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0.85, 1.00, 0.86);
		glVertex3f(312.5, 250, 0);
		glVertex3f(312.5, 245, 0);
		glVertex3f(322.5, 245, 0);
		glVertex3f(322.5, 250, 0);
		glEnd();
		glFlush();
	}
			break;
	case 'r': {
		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(1, 0, 0);
		glVertex3f(185, 270, 0);
		glVertex3f(185, 265, 0);
		glVertex3f(195, 265, 0);
		glVertex3f(195, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1.00, 0.98, 0.83);
		glVertex3f(185, 260, 0);
		glVertex3f(185, 255, 0);
		glVertex3f(195, 255, 0);
		glVertex3f(195, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0.85, 1.00, 0.86);
		glVertex3f(185, 250, 0);
		glVertex3f(185, 245, 0);
		glVertex3f(195, 245, 0);
		glVertex3f(195, 250, 0);
		glEnd();

		//ligths RED
		glBegin(GL_POLYGON);
		glColor3f(1, 0, 0);
		glVertex3f(312.5, 270, 0);
		glVertex3f(312.5, 265, 0);
		glVertex3f(322.5, 265, 0);
		glVertex3f(322.5, 270, 0);
		glEnd();

		//Lights YELLOW
		glBegin(GL_POLYGON);
		glColor3f(1.00, 0.98, 0.83);
		glVertex3f(312.5, 260, 0);
		glVertex3f(312.5, 255, 0);
		glVertex3f(322.5, 255, 0);
		glVertex3f(322.5, 260, 0);
		glEnd();
		//Lights GREEN
		glBegin(GL_POLYGON);
		glColor3f(0.85, 1.00, 0.86);
		glVertex3f(312.5, 250, 0);
		glVertex3f(312.5, 245, 0);
		glVertex3f(322.5, 245, 0);
		glVertex3f(322.5, 250, 0);
		glEnd();
		glFlush();

	}
			break;
	}
}


void main(int argc, char* argv[])
{
	glutInit(&argc, argv);
	glutInitDisplayMode(GLUT_SINGLE | GLUT_RGB);
	glutInitWindowSize(500, 500);
	glutInitWindowPosition(100, 100);
	glutCreateWindow("square");
	glClearColor(0.529412, 0.807843, 0.980392, 0);
	gluOrtho2D(0, 400.0, 0, 500.0);
	glutDisplayFunc(display);
	glutKeyboardFunc(keyDown);
	glutMainLoop();

}