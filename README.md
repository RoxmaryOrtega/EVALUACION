#include <stdio.h>
#include <math.h>
#include <string>
using namespace std;

int main()
{
    int alumno, sumatoria, promedio, reprobados=0, aprobados=0, categoria;
    float prom;
    char letra;
    int nota, c=0;
    char nombre [15];
    int total_alumnos;
    int num_personas=0;
    total_alumnos=15;
    do 
    {
     for (int i = 0; i < total_alumnos; i++)
         {
            printf ( "Introduce el nombre del estudiante:");
            scanf ("%c",&nombre);
            printf( "Introduce su nota:");
            scanf ("%d",&nota);
		     if(nota>20)
             {
             Printf( "no se permiten numeros mayores a 20", endl);
             nota--;
             }
              else
              
             if (nota >= 19)
              {
               letra = "Sobresaliente";
              }
             else if (nota  >= 16)
                {
               letra = "Muy bueno";
                 }
             else if (nota >= 13)
              {
              letra = "Bueno";
              }
              else if (nota >= 10)
             {
             letra = "Regular";
             }
             else if (nota >= 6)
             {
             letra= "Mejorable";
             }
              else 
            {
              letra = "deficiente";
            }
            printf<< "Su clasificacion es: \n" << letra << endl;
        c=c+nota;
        if(nota>=10)
        aprobados++;
        if (nota<10)
        reprobados++;
         } 
    } while (num_personas == total_alumnos);
          
          
          {
          prom=c/total_alumnos;
          printf("-------------------------------------",endl);
          printf ("el promedio de la seccion es:%d \n",prom);
         printf("la cantidad de reprobados es: %d \n", reprobados);
         printf("la cantidad de aprobados es: %d  \n", aprobados);
         printf("Son 15 estudiantes en total", endl);
          }
    return 0;
}
