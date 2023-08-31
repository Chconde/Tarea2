> Tarea 2 Triangulo

# Python

def  imprimir_triangulo_opcion1(num_filas):

for  i  in  range(1, num_filas  +  1):

print('*'  *  i)

  

def  imprimir_triangulo_opcion2(num_filas):

for  i  in  range(num_filas, 0, -1):

print('*'  *  i)

  

def  imprimir_triangulo_opcion3(num_filas):

for  i  in  range(1, num_filas  +  1):

print(' '  * (num_filas  -  i) +  '*'  *  i)

  

def  imprimir_triangulo_opcion4(num_filas):

for  i  in  range(num_filas, 0, -1):

print(' '  * (num_filas  -  i) +  '*'  *  i)

  

def  main():

num_filas  =  int(input("Ingresa un número entero positivo: "))

opcion  =  int(input("Elige una opción de triángulo (1-4):\n"

"1. Triangulo rectangulo izquierdo\n"

"2. Triangulo rectangulo derecho\n"

"3. Triangulo rectangulo izquierdo invertido\n"

"4. Triangulo rectangulo derecho invertido\n"

"Opción: "))

  

if  opcion  ==  1:

imprimir_triangulo_opcion1(num_filas)

elif  opcion  ==  2:

imprimir_triangulo_opcion2(num_filas)

elif  opcion  ==  3:

imprimir_triangulo_opcion3(num_filas)

elif  opcion  ==  4:

imprimir_triangulo_opcion4(num_filas)

else:

print("Opcion no válida. Debes elegir una opcion del 1 al 4.")

  

if  __name__  ==  "__main__":

main()

# C++

#include <iostream>
using namespace std;

void imprimir_triangulo_opcion1(int num_filas) {
    for (int i = 1; i <= num_filas; ++i) {
        for (int j = 0; j < i; ++j) {
            cout << '*';
        }
        cout << endl;
    }
}

void imprimir_triangulo_opcion2(int num_filas) {
    for (int i = num_filas; i >= 1; --i) {
        for (int j = 0; j < i; ++j) {
            cout << '*';
        }
        cout << endl;
    }
}

void imprimir_triangulo_opcion3(int num_filas) {
    for (int i = 1; i <= num_filas; ++i) {
        for (int j = 0; j < num_filas - i; ++j) {
            cout << ' ';
        }
        for (int j = 0; j < i; ++j) {
            cout << '*';
        }
        cout << endl;
    }
}

void imprimir_triangulo_opcion4(int num_filas) {
    for (int i = num_filas; i >= 1; --i) {
        for (int j = 0; j < num_filas - i; ++j) {
            cout << ' ';
        }
        for (int j = 0; j < i; ++j) {
            cout << '*';
        }
        cout << endl;
    }
}

int main() {
    int num_filas, opcion;
    
    cout << "Ingresa un numero entero positivo: ";
    cin >> num_filas;
    
    cout << "Elige una opción de triángulo (1-4):\n"
         << "1. Triangulo rectangulo izquierdo\n"
         << "2. Triangulo rectangulo derecho\n"
         << "3. Triangulo rectangulo izquierdo invertido\n"
         << "4. Triangulo rectangulo derecho invertido\n"
         << "Opcion: ";
    cin >> opcion;
    
    switch (opcion) {
        case 1:
            imprimir_triangulo_opcion1(num_filas);
            break;
        case 2:
            imprimir_triangulo_opcion2(num_filas);
            break;
        case 3:
            imprimir_triangulo_opcion3(num_filas);
            break;
        case 4:
            imprimir_triangulo_opcion4(num_filas);
            break;
        default:
            cout << "Opcion no valida. Debes elegir una opción del 1 al 4." << endl;
            break;
    }

    return 0;
}

# Pseudocodigo

Algoritmo Triangulo
	Imprimir "Ingrese un número entero positivo:"
	Leer num_filas
	
	Imprimir "Elige una opción de triángulo (1-4):"
	Imprimir "1. Triangulo rectangulo izquierdo"
	Imprimir "2. Triangulo rectangulo derecho"
	Imprimir "3. Triangulo rectangulo izquierdo invertido"
	Imprimir "4. Triangulo rectangulo derecho invertido"
	Leer opcion
	
	Según opcion Hacer
Caso 1:
	Para i desde 1 hasta num_filas Hacer
		Para j desde 1 hasta i Hacer
			Imprimir "*"
		Fin Para
		Imprimir Nueva Línea
	Fin Para
Caso 2:
	Para i desde 1 hasta num_filas Hacer
		Para j desde 1 hasta num_filas - i Hacer
			Imprimir " "
		Fin Para
		Para j desde 1 hasta i Hacer
			Imprimir "*"
		Fin Para
		Imprimir Nueva Línea
	Fin Para
Caso 3:
	Para i desde 1 hasta num_filas Hacer
		Para j desde 1 hasta i - 1 Hacer
			Imprimir " "
		Fin Para
		Para j desde i hasta num_filas Hacer
			Imprimir "*"
		Fin Para
		Imprimir Nueva Línea
	Fin Para
Caso 4:
	Para i desde 1 hasta num_filas Hacer
		Para j desde 1 hasta num_filas - i Hacer
			Imprimir " "
		Fin Para
		Para j desde 1 hasta i Hacer
			Imprimir "*"
		Fin Para
		Imprimir Nueva Línea
	Fin Para
De Otro Modo:
	Imprimir "Opcion no valida. Debes elegir una opción del 1 al 4."
Fin Según



FinAlgoritmo
