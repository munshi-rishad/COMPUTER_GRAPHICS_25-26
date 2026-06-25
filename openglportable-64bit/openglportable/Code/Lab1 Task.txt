#include <GL/glut.h>
#include <cmath>

void display()
{
    glClear(GL_COLOR_BUFFER_BIT);
////1st
//      glBegin(GL_LINES);
//
//
//        glVertex2f(0,-0.4);
//        glVertex2f(0, 0.4);
//
//        glVertex2f(-0.5, 0.2);
//       glVertex2f(0.5, 0.2);
//
//
//       glVertex2f(0,-0.4);
//       glVertex2f(-0.4,-0.8);
//
//       glVertex2f(0,-0.4);
//       glVertex2f(0.4,-0.8);
//
//
//        glEnd();
//        glBegin(GL_LINE_LOOP);
//        for(float theta=0; theta<=2*3.14; theta=theta+0.001){
//            glVertex2f(sin(theta)*0.3,(cos(theta)*0.3)+0.69);
//        }
//2nd
//glBegin(GL_LINES);
//       glVertex2f(-0.5, 0);
//       glVertex2f(0.5, 0);
//
//      glVertex2f(0.5, 0);
//       glVertex2f(0.5, 0.5);
//
//       glVertex2f(0.5, 0.5);
//      glVertex2f(-0.5, 0.5);
//
//
//       glVertex2f(-0.5, 0.5);
//       glVertex2f(-0.5, 0);
//
//       glVertex2f(0, 0.9);
//       glVertex2f(-0.5, 0.5);
//
//       glVertex2f(0, 0.9);
//        glVertex2f(0.5, 0.5);
//
//        glVertex2f(-0.1, 0);
//        glVertex2f(-0.1, 0.2);
//
//        glVertex2f(-0.1, 0.2);
//        glVertex2f(0.1, 0.2);
//
//        glVertex2f(0.1, 0.2);
//        glVertex2f(0.1, 0);
//
//3rd

        glBegin(GL_LINES);


        glVertex2f(-0.5, -0.2);
       glVertex2f(0.5, -0.2);

       glVertex2f(0.5, -0.2);
      glVertex2f(0.5, 0.2);

      glVertex2f(0.5, 0.2);
       glVertex2f(-0.5, 0.2);

       glVertex2f(-0.5, 0.2);
       glVertex2f(-0.5, -0.2);


       glVertex2f(-0.1, 0.2);
       glVertex2f(-0.1, 0.4);

       glVertex2f(0.1, 0.2);
       glVertex2f(0.1, 0.4);

        glEnd();
        glBegin(GL_LINE_LOOP);
        for(float theta=0; theta<=2*3.14; theta=theta+0.001){
            glVertex2f(sin(theta)*0.3,(cos(theta)*0.3)+0.69);
        }


    glEnd();
    glFlush();
}

int main(int argc, char** argv)
{
    glutInit(&argc, argv);
    glutInitWindowSize(800, 800);
    glutCreateWindow("OpenGL 64bit");
    glutDisplayFunc(display);
    glClearColor(0.0f, 0.0f, 0.0f, 1.0f);
    glutMainLoop();
    return 0;
}
