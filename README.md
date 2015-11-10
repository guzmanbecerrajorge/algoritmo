# algoritmo
#include "stdafx.h"
#include "conio.h"
#include <iostream>

using namespace std;
#define fil 50
#define col 50

void cargar(int mat[fil][col],int x, int y);
void mostrar(int mat[fil][col],int x, int y);
void clasificarBurbuja(int mat[fil][col],int x,int y,int aux);

void main()
{int a,b,mat[fil][col],opcion;
do
{cout<<" MENU";
 cout<<"1. Cargar matriz"<<endl;
 cout<<"2. Mostrar matriz"<<endl;
 cout<<"3. Clasificar matriz"<<endl;
 cout<<"4. Clasificar burbuja"<<endl;
 cout<<"0. SALIR"<<endl;
 cout<<"Ingrese opcion: ";
 cin>>opcion;
 switch(opcion)
 {case 1: do{ cout<<"ingresar el numero de filas: ";
		  cin>>a;
		  } while(a>ROW);
          do {cout<<"ingresar el numero de columnas: ";
		  cin>>b;
		  } while(b>COL);
		  cargar(mat,a,b);
		  break;
  case 2: mostrar(mat,a,b);
	      break;
  case 3: clasificarBurbuja(mat,a,b);
	      break;
  case 0: cout<< "Gracias";
	      break;
  default: cout<<"Ingrese opcion valida";
		  break;
 } while(opcion!=0);
getch();	
}

void cargar(int mat[fil][col],int x, int y)
{for(int i=0;i<x;i++)
	{for(int k=0;k<y;k++)
		{cout<<"mat["<<i<<"]["<<k<<"]: ";
		cin>>mat[i][k];
		}
	}
}

void mostrar(int mat[fil][col],int x, int y)
{for(int i=0;i<x;i++)
	{cout<<endl;
	for(int k=0;k<y;k++)
		cout<<mat[i][k]<<"\t";
		
	}
}

void clasificarBurbuja(int mat[fil][col],int x, int y,int aux)
{int i,j;
  for(i=0;i<n;i++)
  {for(j=o;j<m;j++)
  {if(mat[i][j]>mat[j][i])
  {aux=mat[i][j];
  mat[i][j]=mat[j][i];
  mat[j][i]=aux;
  }
  }
  }
}

    Status API Training Shop Blog About Pricing 

    © 2015 GitHub, Inc. Terms Privacy Security Contact Help 
