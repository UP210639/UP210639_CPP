
# Codigos De La Unidad 2

![screenshot](https://github.com/UP210639/UP210639_CPP/blob/main/Recursos/Elma.jpg)  

# Unidad 2 
**Alfabeto**
````
#include <iostream>
#include <stdio.h>

using namespace std;

int main ()
{
    char A = 65;
    char a ='Z';
    int n=0;
    cout << "Alfabeto Mayuscula A-Z" << endl;
    for (char A = 65; A <= 90 ; A++)
    {
       cout << A << endl;
    }
    cout << "Alfabeto Mayuscula Z-A" << endl;
    
    for (int i = 0; i <= 26; i++)
    {
        cout << a << endl;
        a=a-1;
    }
    cout << "Numeros del 1 al 10" << endl;
    for (int n = 0; n <= 10; n++)
    {
        cout << n << endl;
    }
    return 0;   
}

````
---
**Tramos**
````
#include <iostream>
#include <iomanip>
#include <string>
using namespace std;

int main () 
{ 
   int R;
   int t;
   int T;
   cout << "Cual es el monto de tu renta \n";
   cin >> R;
   if (R >=0 && R <= 65000)
    {
        if (R < 10000 ) {
            printf("Impuesto a pagar de 5%\n");
            t=R*.05;
            T=R+t;
            cout << "Total a pagar" << T << endl;
            
        }

        else if (R >= 10000 && R < 20000) {
            printf("Impuesto a pagar de 15%\n");
            t=R*.15;
            T=R+t;
            cout << "Total a pagar" << T << endl;
            
        }
        else if (R >= 20000 && R < 35000) {
            printf("Impuesto a pagar de 20%\n");
            t=R*.2;
            T=R+t;
            cout << "Total a pagar" << T << endl;
            
        }
        else if (R >= 35000 && R < 60000) {
            printf("Impuesto a pagar de 30%\n");
            t=R*.3;
            T=R+t;
            cout << "Total a pagar" << T << endl;
            
        }
        else {
            printf("Impuesto a pagar de 45%\n");
            t=R*.45;
            T=R+t;
            cout << "Total a pagar" << T << endl;
        }
    }
    else
        printf("No pagas impuesto\n");

    return 0;
}
````
---
**Beneficios**
````
#include <iostream>
#include <iomanip>
#include <string>
using namespace std;

int main()
{
    float p = 40;
    float P=0;
    float r=0;
    char rendimiento = 'I';

    cout << "Bienvenido, Inserte la puntacion del empleado"; //Toma valores enteros y dentro del programa ya lo trasforma a punto decimal 
    cin >> p;

    if (p == 0)
    {
        rendimiento = 'I';
        if (p == 0 || p == 40 || p >= 60)

            P = p / 100; //Aqui cambia el valor con puntod decimal 
            r = P * 2400; 

             cout << "\n El rendimiento del empleado es: " << rendimiento << " \n Recibira :" << r;
    }
    else if (p == 40)
    {
        rendimiento = 'A';
        if (p == 0 || p == 40 || p >= 60)

            P = p / 100;
            r = P * 2400;

            cout << "\n El rendimiento del empleado es: " << rendimiento << " \n Recibira :" << r;
    }
    else if (p >= 60)
    {
        rendimiento = 'M';
        if (p == 0 || p == 40 || p >= 60)

            P = p / 100;
            r = P * 2400;

            cout << "\n El rendimiento del empleado es: " << rendimiento << " \n Recibira :" << r;
    }
    else
        cout << "\n No califica";

    return 0;
}
````
---
**Entradas**
````
#include <iostream>
#include <iomanip>
#include <string>
using namespace std;

int main () 
{
    int e=5;
    cout << "Bievenido \n" << "¿Cuantos años tienes? \n";
    cin >> e;
    if (e < 4)
    { 
        int p=0;
        cout << "\n Bienvenido";
    }
    else if  (e >= 4 && e <= 18)
    { 
        int p=5;
        cout << "\n Paga " << p << "\n Bienvenido :D";
    }
    else if (e > 18)
    { 
        int p=10;
        cout << "\n Paga" << p << "\n Bienvenido :D";
    }

    else 

    cout << ("\n Vuelva pronto");

    return 0;

}
````
---
**Pizzeria**
````
include <iostream>
#include <stdlib.h>

using namespace std;

int main()
{
    int P = 1;
    int I = 2;

    cout << "Bienvenido a pizza Bella Napoli \n" << "Que va a llevar? 1=Vegetariana 0=Tradicional";
    cin >> P;

    if (P == 1)
    {
        cout << "Que ingrediente extra desea agregar? \n";
        cout << "Menu \n"
             << "1 = Pimiento, 2 = tofu \n";
        cin >> I;

        if (I == 1)
        {
            cout << "Su orden es: Un Pizza Vegetariana con Pimiento \n";
            cout << "Espero la disfrute :D \n";
        }
        else
            cout << "Su orden es: Un Pizza Vegetariana con Tofu \n";
        cout << "Espero la disfrute :D \n";
    }

    else if (P == 0) 

    {
        cout << "Que ingrediente extra desea agregar? \n";
        cout << "Menu \n"
             << "1 = Jamon, 2 = Peperoni, 3 = Salmon \n";
        cin >> I;

        if (I == 1)
        {
            cout << "Su orden es: Un Pizza Tradicional con Jamon \n";
            cout << "Espero la disfrute :D \n";
        }
        else if (I == 2)
        {
            cout << "Su orden es: Un Pizza Tradicional con Peperoni \n";
            cout << "Espero la disfrute :D \n";
        }
        else
            cout << "Su orden es: Un Pizza Tradicional con Salmon \n";
        cout << "Espero la disfrute :D \n";
    }

    else 

    cout << "VUelva pronto \n";
    
    return 0;
}
````
---
**Temperaturas**
````
#include <iostream>
#include <stdlib.h>

using namespace std;

int main()
{
    int temperatura, sumatoria, mayor, menor;
    for (int i = 1; i <= 6; i++)
    {
        cout << "Ingresar la temperatura " << i;
        cin >> temperatura;
        sumatoria = sumatoria + temperatura;
        if (i == 1)
        {
            mayor = temperatura;
            menor = temperatura;
        }
        else
        {
            if (temperatura > mayor)
            {
                mayor = temperatura;
            }
            else
            {
                if (temperatura < menor)
                {
                    menor = temperatura;
                }
            }
        }
    }
    cout << "El promedio de las 6 temperaturas es:" << sumatoria / 6;
    cout << "La  temperatura mas grande es: " << mayor;
    cout << "La  temperatura mas pequeña es: " << menor;

    return 0;
}
````
---
**SuperMercado**
````
#include <iostream>
#include <stdlib.h>

using namespace std;

int main()
{
    int c=0;
    int p=0;
    int t=0;
    int s=0;

    do
    {
        cout << "Cantidad de productos \n";
        cin >> c;
        cout << "Precio por unidad \n";
        cin >> p;

        s = c * p;

        t = t + s;

    } while ( c != 0);

    cout << "\n El total a pagar es: " << t;
    cout << "vuelva pronto :D \n";
    
    return 0;

}
````
---
**Binario a decimal**
````

unsigned long long binarioADecimal(char *cadenaBinaria, int longitud);

int main()
{

    char binario[LONGITUD_MAXIMA];
    printf("Introduce un número binario de hasta %d caracteres:\n",
           LONGITUD_MAXIMA - 1);
    fgets(binario, LONGITUD_MAXIMA, stdin);
    binario[strcspn(binario, "\r\n")] = 0;

    unsigned long long decimal = binarioADecimal(binario, strlen(binario));
    printf("El binario %s es %llu en decimal", binario, decimal);
    return 0;
}

unsigned long long binarioADecimal(char *cadenaBinaria, int longitud)
{
    unsigned long long decimal = 0;
    int multiplicador = 1;
    char caracterActual;
    for (int i = longitud - 1; i >= 0; i--)
    {
        caracterActual = cadenaBinaria[i];
        if (caracterActual == '1')
        {
            decimal += multiplicador;
        }
        multiplicador = multiplicador * 2;
    }
    return decimal;
}

````