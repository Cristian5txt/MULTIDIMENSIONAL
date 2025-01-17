#include <iostream>
#include  <string>

using namespace std;

int main()
{
     int dimension,fila,columna;
    cout<< "INGRESE EL NUMERO DE MATRICES"<<endl;
    cin>>dimension;
    cout<< "INGRESE EL NUMERO DE FILAS"<<endl;
    cin>>fila;
    cout<< "INGRESE EL NUMERO DE COLUMNAS"<<endl;
    cin>>columna;



    int notasP1[dimension][fila][columna];

    //INGRESAR
    for (int a=0;a<dimension;a++){
        for (int i=0;i<fila;i++){
            for (int j=0;j<columna; j++){
    cout << "INGRESE LAS NOTAS: "<< "["<<a<<"]["<<i<<"]["<<j<<"]"<<endl;
    cin>> notasP1[a][i][j];
            }
        }
    }

    //IMPRIMIR
    for (int a=0;a<dimension;a++){
        for (int i=0;i<fila;i++){
            for (int j=0;j<columna; j++){
    cout << notasP1[a][i][j]<<" ";
            }
            cout<<endl;
        }
        cout<<endl;
    }

    //CALCULO
    float p1,p2,p3;
    float pt;
    p1= (notasP1[0][0][0]+notasP1[0][0][1]+notasP1[0][0][2]+notasP1[0][0][3]+notasP1[0][0][4]+notasP1[0][0][5])/columna;
    cout<< "SU VALOR TOTAL ES: "<<p1<<endl;

    p2= (notasP1[1][0][0]+notasP1[1][0][1]+notasP1[1][0][2]+notasP1[1][0][3]+notasP1[1][0][4]+notasP1[1][0][5])/columna;
    cout<< "SU VALOR TOTAL ES: "<<p2<<endl;

    p3= (notasP1[2][0][0]+notasP1[2][0][1]+notasP1[2][0][2]+notasP1[2][0][3]+notasP1[2][0][4]+notasP1[2][0][5])/columna;
    cout<< "SU VALOR TOTAL ES: "<<p3<<endl;

    pt= (p1+p2+p3)/3;
    cout<< "SU PARCIAL TOTAL ES: "<<pt<<endl;

    return 0;
}
