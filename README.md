# Lab_assigment_8

#include <iostream>

#include<stdio.h>

#include <stdlib.h>

 

using namespace std;

//Initializing three global 2D array

int MultiArray[8][8];
int MultiArray1[32][32];
int MultiArray2[128][128];

//First function using a 2D array of size [8][8]

int linearIndex(){

    int X[20]; //Initializing a 1D array that will recieve elements from our 2D array.

    int s=-1; //Initializing the index of my 1D array

    int array[8][8],i,j; // Initializing  a local 2D array

    for(i=0;i<8;i++){

        for(j=0;j<8;j++){

             if(i>=j){

            array[i][j]=rand() % 100+1;

            s++;

            X[s]=array[i][j];

            cout <<" " <<"A[" << i<<" ]"<<"["<<j<<"]: "  ;

            cout<<array[i][j] << " ";

            

            MultiArray[i][j]=X[s];

        }  

    }

    

    cout<< endl;

    } 

    cout << "The number of elements is ";

    cout<<s+1 <<endl;

 

    for(int ii=0;ii<20;ii++) {

        cout<<X[ii] << " " ;

 

        cout <<" Is at index: " <<"B [" << ii << " ]" <<endl ;

 

    }   

    cout<< endl;   

}

 

void inverseIndex(){

    for(int i=0;i<8;i++){

        for(int j=0;j<8;j++){

             if(i>=j){

            

            cout <<MultiArray[i][j] <<" ";

            cout <<" Is at index: " <<"C [" << i<<" ] "<<"["<<j<<"]" <<endl ;

             }

        } 

        cout<< endl; 

    }

 

}

 

int main(){

    linearIndex();

    cout<< endl;

    inverseIndex();

    

}
