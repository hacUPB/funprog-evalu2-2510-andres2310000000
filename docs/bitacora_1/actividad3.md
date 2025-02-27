Algoritmos

1. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

```
 Inicio 
 Escribir "cantidad de lapices a llevar"
 leer cantidad
   si cantidad>=1000
   precio=85
   si no
   precio=90 
   fin si
 total=cantidad*precio
 mostrar"serian:",total
 fin 
```  
![alt text](image.png)

2. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.  

```
 Inicio 
 Escribir "precio a pagar:"
 leer precio
   si precio>=250000
   descuento= precio*15/100
   si no
   descuento= precio*8/100
   fin si
  total=precio-descuento
  mostrar" su descuento es de:",descuento
  mostrar"precio con descuento aplicado:",total
 fin 
```    
![alt text](image-1.png)  

3. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.  

```
 Inicio 
 Escribir "numero de alumnos:"
 leer numero
   si numero >=100
   precio=65
   si no
   si numero >=50
   precio=70
   si numero >=30
   precio=95
    si numero es <=29
   precio=4000
   mostrar"precio:4000" 
   fin si
   total=numero*precio
   mostrar"el total es:", total
   fin
```        
![alt text](i2.png)  
  

ejemplo 4.5
```
inicio 
escribir "estatura"
suma=0
num_per=0
estatura=1
mientras estatura > 0
 leer estatura
 mientras estatura > 0
 leer estatura
 si estatura > 0
 suma=suma+estatura
 num_per=num_per+1
 fin mientras
si num_per diferente de 0
prom=suma/num_per
Escribir prom
fin 
```    

  

2.    
```
inicio
escriba"ingrese la cantidad de tela en metros:"
leer tela
map=tela/0.0254
mostrar" la cantidad en puelgadas es:",map
fin
```  

3.  
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

4.  
```
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

5.  
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
      pago=(40*pagoph) + ((horast-40)*(2*pagoph))
    si horast <= 50 
      pago=(40*pagoph)+          (5*(2*pagoph))+((horast - 45)*(3*pagoph))
    fin Si
mostrar "El sueldo semanal es: ", sueldo
fin
```    
6.  
```
innicio
escriba"ingrese numeros:"
n=0
p=0
ne=0
si numeros=0
 ne=ne+1
si numeros>0
 p=p+1
si no
 n=n+1 
 fin si
 mostrar "los 0 son:",ne
 mostrar "los p son:",p
 mostrar "los n son:",n
fin 
```
7.  
```
incio
n=3
x=1
acum=0
mientras x<=365
hacer
x=x+1
a=3^x
acum=a+acum
mostrar"el total ahorrdo si se sigue la secuenca es:",acum
fin
```
8.  
```
imicio
fin
```
   
  

   
