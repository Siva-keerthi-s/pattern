//When time is the constraint it is the best option, but take some time and challenge your brain
/* lets print this pattern  
    1
   121    Siva Keerthi
  12321
 1234321  */
#include <iostream>
using namespace std;
int main(){

int i,j,k,y,row = 4,column = 4,num = 1;
    for ( i = 0; i < row; i++){
        for(j = 0; j < column - i; j++){
            cout << " ";
        }     
        for(k = 1; k <= i; k++){
            cout << k;
        }
        
        for(y = i+1; y >0; y-- ){
            cout << y; 
        }
        cout << "\n";
    }
    return 0;
{
