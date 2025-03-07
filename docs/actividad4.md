1. ¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en C?  

    Porque nos ayuda a resolver el problema en nuestra mente y luego asi poder realizar el pseudocodigo, para que se vuelva más sencillo y finalmente que simplemente sea usar los comandos de programacion en c o en cualquier otro lenguaje. 

2. Toma un pseudocódigo de un ejercicio anterior o escribe tu propio pseudocódigo, similar al mostrado en el ejemplo de arriba.  
```
inicio
ingrese x1 , y1
leer x1 , y1
ingrese x2 , y2
leer x2 , y2

calculo SQRT((x2-x1)^2+(y2-y1)^2)
mostrar "la distancia es",calculo
fin
```
3. ¿Por qué es importante declarar el tipo de variable (int, float, etc.) antes de usarla en C?
Porque siempre antes de empezar un codigo ees necesario declarar el tipo de variables que se van a usar , lo que implica que cada variable debe tener un tipo de dato definido en tiempo de compilación. Esto permite que el compilador asigne correctamente la memoria requerida, optimice la ejecución del código y realice verificaciones de tipo para prevenir errores en tiempo de compilación. 

4. Actividad:    
```
Inicio
    Escriba "Ingrese la cantidad de calificaciones: "
    Leer n
    sumatotal=0
    Para i desde 1 hasta n
     Escriba "Ingrese la calificación ", i, ": "
     Leer calificacion
     sumatotal=sumatotal+calificacion
    Fin Para
    promedio=sumatotal/n
    mostrar "Promedio:", promedio
Fin  
```     
codigo en C:  
```
#include <stdio.h>

int main() {
    int n, i;
    float calificacion, sumatotal=0, promedio;

    printf("Ingrese la cantidad de calificaciones: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
     printf("Ingrese la calificación %d: ", i);
     scanf("%f", &calificacion);
     sumatotal+=calificacion;
    }
    promedio=sumatotal/n;
    printf("El promedio es: %.d\n", promedio);

    return 0;
}
```

5.  ¿Por qué es importante comentar el código, aunque sea breve y conciso?
Porque ayudan a entender mucho mas facil el codigo y esto ahorra demasiado tiempo a la persona que lo hace como a la persona que lo revisa.  

6. 

6.1.  

Pseudocodigo
 ```
inicio
escriba" x1 , y1"
leer x1 , y1
escriba" x2 , y2"
leer x2 , y2

calculo SQRT((x2-x1)^2+(y2-y1)^2)
mostrar "la distancia es",calculo
fin
 ``` 
Codigo en c
```
#include <stdio.h>
#include <math.h>  

int main() {
    float x1, y1, x2, y2, distancia;

    // Solicitar los puntos al usuario
    printf("Ingrese x1: ");
    scanf("%f", &x1);
    
    printf("Ingrese  y1: ");
    scanf("%f",&y1);
    
    printf("Ingrese x2: ");
    scanf("%f", &x2);
    
       printf("Ingrese  y2: ");
    scanf("%f",&y2);

    // Cálculo de la distancia usando la fórmula
    distancia = sqrt(pow(x2-x1, 2) + pow(y2-y1, 2));

    // Mostrar el resultado
    printf("La distancia es: %.2f\n", distancia);

    return 0;
}
```
6.2  
Pseudocodigo:  
```
inicio
escriba"ingrese la cantidad de tela en metros:"
leer tela
map=tela/0.0254
mostrar" la cantidad en puelgadas es:",map
fin
```    
Codigo en C
```
#include <stdio.h>

int main() {
    float tela, pulgadas;

    printf("Ingrese la cantidad de tela en metros: ");
    scanf("%f", &tela);


    pulgadas=tela/0.0254;

    printf("La cantidad en pulgadas es: %.2f\n", pulgadas);

    return 0;
}
```
6.3.  
Pseudocodigo: 
```
inicio
escriba"ingrese cateto_ad:"
leer cateto_ad
escriba"ingrese cateto_op:"
leer cateto_op
h=SQRT(cateto_ad^2+cateto_op^2)
mostrar" la hipotenusa es:",h
fin
```      
Codigo en C
```
#include <stdio.h>
#include <math.h>  // Necesario para sqrt()

int main() {
    float cateto_ad, cateto_op, h;
    
    printf("Ingrese cateto adyacente: ");
    scanf("%f", &cateto_ad);
    
    printf("Ingrese cateto opuesto: ");
    scanf("%f", &cateto_op);

    h = sqrt(pow(cateto_ad, 2) + pow(cateto_op, 2));
    
    printf("La hipotenusa es: %.2f\n", h);

    return 0;
}
```
6.4.
incio
escriba "ingresar año_a actual:"
escriba "ingresar mes_a actual:"
escriba "ingresar dia_a actual:"
leer año_a
leer mes_a
leer dia_a
escriba "ingresar año de nacimiento:"
escriba "ingresar mes de nacimiento:"
escriba "ingresar dia de nacimiento:"
leer año
leer mes
leer dia

a=año_a-año
si mes<mes_a
   a=a-1
   mostrar"usted no ha cumplido años, edad:",a
si mes=mes_a
 hacer
 si dia>dia_a
  mostrar"usted ya cumplio años, edad",a
 si dia=dia_a
 mostrar"feliz cumpleaños, edad:",a
  si no
  mostrar"usted no ha cumplido años, edad",a
    
si no
  mostrar"usted ya cumplio años, edad",a
fin si
fin
```    
Codigo en C
```
#include <stdio.h>

int main() 
{
    int año_a, mes_a, dia_a;  
    int año, mes, dia;        
    int edad;

    printf("Ingresar año actual: ");
    scanf("%d", &año_a);
    
    printf("Ingresar mes actual: ");
    scanf("%d", &mes_a);
    
    printf("Ingresar día actual: ");
    scanf("%d", &dia_a);

    printf("Ingresar año de nacimiento: ");
    scanf("%d", &año);
    
    printf("Ingresar mes de nacimiento: ");
    scanf("%d", &mes);
    
    printf("Ingresar día de nacimiento: ");
    scanf("%d", &dia);

    edad = año_a - año;

    if (mes > mes_a || (mes == mes_a && dia > dia_a)) 
    {
        edad -= 1;
        printf("Usted no ha cumplido años, edad: %d\n", edad);
    } 
    
    else if (mes == mes_a && dia == dia_a) 
    {
        printf("¡Feliz cumpleaños! Edad: %d\n", edad);
    } 
    
    else 
    {
        printf("Usted ya cumplió años, edad: %d\n", edad);
    }

    return 0;
}
```
6.5.  
Pseudocodigo: 
```
inicio
    ecriba "Ingrese las horas trabajadas en la semana: "
    leer horast
    escriba "Ingrese el pago por hora: "
    leer pagoph

    si horast > 50 
      Escribir "No se permite trabajar más de 50 horas."
    si no
      pago=0
    si horast <= 40 
      sueldo=horast*pagoph
    si 
      horast <= 45 
      sueldo=(40*pagoph)+((horast-40)*(2*pagoph))
    si horast <= 50 
      sueldo=(40*pagoph)+(5*(2*pagoph))+((horast - 45)*(3*pagoph))
    fin si
mostrar "El sueldo semanal es: ", sueldo
fin
```   
Codigo en C
```
#include <stdio.h>

int main() 
{
    int horast;
    float pagoph, sueldo = 0;

    printf("Ingrese las horas trabajadas en la semana: ");
    scanf("%d", &horast);
    printf("Ingrese el pago por hora: ");
    scanf("%f", &pagoph);

    if (horast > 50) 
    {
        printf("No se permite trabajar más de 50 horas.\n");
    } 
    else {
          if (horast <= 40) 
           {
            sueldo = horast * pagoph;
           } 
           else if (horast <= 45) 
           {
            sueldo = (40 * pagoph) + ((horast - 40) * (2 * pagoph));
           } 
           else if (horast <= 50) 
           {
            sueldo = (40 * pagoph) + (5 * (2 * pagoph)) + ((horast - 45) * (3 * pagoph));
           }
        printf("El sueldo semanal es: %.2f\n", sueldo);
         }

    return 0;
}
```   

Después de este tutorial, ¿qué puntos crees que deberías reforzar para sentirte más seguro al traducir pseudocódigo a C?  
usar mejor los for y aprender las formulas que se pueden hacer en este lenguaje de programación, y seguir practicando. 
