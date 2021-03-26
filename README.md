# Lab_assigment_8

#include <iostream>
#include <stdio.h>
#include <stdlib.h>


using namespace std;

int main(){
    
    int x [7] [7], i , j;
    int y [49], a = 1, b = 0;
    
    for (i = 0; i< 7; i++){
        
        for (j = 0; j< 7;j++){
            
            x [i][j] = rand() % 100;
            
    }
    }
      cout << "the Lower triangular is ...." << endl;
    for (i = 0; i< 7; i++){
        
        for (j = 0; j< 7;j++){
            
            if (i>j){
            
            cout << x[i][j] << " "; 
            
            }
}
        cout<< endl;
}
