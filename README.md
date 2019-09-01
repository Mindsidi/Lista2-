# Lista2
//Constante de kapetar ,kaprekar

#include <stdio.h>

int main(void) {

int  numero=0,x=0,y=0,z=0,k=0,cresc1=0,cresc2=0,cresc3=0,cresc4=0,decres1=0,decres2=0,decres3=0,decres4=0,numero1=0,numero2=0,gatilho=0;
 
 printf("digite um numero de 4 digitos de 2 digitos diferentes\n");
   scanf("%d", &numero);


 while(numero!=6174){

 
   x=numero/1000;
   y=(numero/100)-(x*10);
   z=(numero/10)-((x*100)+(y*10));
   k=(numero/1)-((x*1000)+(y*100)+(z*10));

   //printf("\n%d %d %d %d", x,y,z,k);
  //----------------------------------------------------------
//1

if(x<y && x<z && x<k){

      cresc1=x;
      decres4=x;
//y
    if(y<z && y<k){

        cresc2=y;
        decres3=y;
   
       if(z<k){

            cresc3=z;
            decres2=z;

            cresc4=k;
            decres1=k;     }

       if(k<z){


            cresc3=k;
            decres2=k;

            cresc4=z;
            decres1=z;

       }

      }
//z
      if(z<y&&z<k){

        cresc2=z;
        decres3=z;

          if(y<k){

            cresc3=y;
            decres2=y;

            cresc4=k;
            decres1=k;
         }

          if(k<y){

            cresc3=k;
            decres2=k;

            cresc4=y;
            decres1=y;         }

      }

//k     
      if(k<y&&k<z){

         cresc2=k;
         decres3=k;

           if(y<z){

              cresc3=y;
              decres2=y;

              cresc4=z;
              decres1=z;             

           }

            if(z<y){

              cresc3=z;
              decres2=z;

              cresc4=y;
              decres1=y;      
        }

//---------------------------------------------------------------


  }
  
//2
if(y<x && y<z && y<k){

      cresc1=y;
      decres4=y;
//x
    if(x<z && x<k){

        cresc2=x;
        decres3=x;
   
       if(z<k){

            cresc3=z;
            decres2=z;

            cresc4=k;
            decres1=k;     }

       if(k<z){


            cresc3=k;
            decres2=k;

            cresc4=z;
            decres1=z;

       }

      }
//z
      if(z<y&&z<k){

        cresc2=z;
        decres3=z;

          if(y<k){

            cresc3=y;
            decres2=y;

            cresc4=k;
            decres1=k;
         }

          if(k<y){

            cresc3=k;
            decres2=k;

            cresc4=y;
            decres1=y;         }

      }

//k     
      if(k<y&&k<z){

         cresc2=k;
         decres3=k;

           if(y<z){

              cresc3=y;
              decres2=y;

              cresc4=z;
              decres1=z;             

           }

            if(z<y){

              cresc3=z;
              decres2=z;

              cresc4=y;
              decres1=y;      
        }

  }}
//3
if(z<y && z<x && z<k){

      cresc1=z;
      decres4=z;

    if(y<z&&y<k){

        cresc2=y;
        decres3=y;

    }

  }
//4
if(k<y && k<z && k<x){

      cresc1=k;
      decres4=k;

    if(y<z&&y<k){

        cresc2=y;
        decres3=y;

    }

  }


//--------------------------------------------------

 }
  printf(" \nVolte sempre\n");

  return 0;
}
