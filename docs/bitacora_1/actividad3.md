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
  