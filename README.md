# NumerosComplejosFlex

# Requerimiento

El programa requiere los siguientes archivos ubicados en la misma carpeta:

numeros_complejos.l

entrada.txt

El archivo entrada.txt debe contener al menos una línea.
Cada línea representa una cadena que será evaluada por el analizador léxico para verificar si tiene la forma:

a+bi
a-bi


Donde:

a y b ∈ ℝ (números reales)

i puede ser i, I, j, J

2️⃣ Requisitos del sistema

Tener instalado:

Flex

GCC (compilador de C)

En Linux se puede instalar con:

sudo apt install flex gcc

3️⃣ Abrir la terminal

Abrir la terminal del sistema operativo.

4️⃣ Navegar hasta la carpeta del programa

Usar el comando cd para ubicarse en la carpeta donde están los archivos:

cd ruta/de/la/carpeta


Ejemplo:

cd Documentos/AnalizadorComplejos

5️⃣ Compilar el programa

Ejecutar los siguientes comandos:

flex numeros_complejos.l
gcc lex.yy.c -o complejos -lfl


Esto generará el ejecutable llamado complejos.

6️⃣ Ejecutar el programa

Una vez compilado, ejecutar:

./complejos entrada.txt


El comando ejecuta el programa y utiliza el archivo entrada.txt como entrada.

7️⃣ Salida del programa

El programa mostrará el resultado en la consola:

ACEPTA


o

NO ACEPTA


Esto indica si la cadena del archivo cumple o no con el formato de número complejo definido.

📌 Ejemplo de entrada válida
3+4i
-2.5-7.8J
0+3j

📌 Ejemplo de entrada no válida
3+i
4j+5
3++4i
