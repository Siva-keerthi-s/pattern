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
// Hallo Diamond
#include <iostream>
using namespace std;
int main(){
    int i,j,k,row = 5,column = 5,num = 1;
    for(i = 0; i<row; i++){
        for(j  = 0; j< column - i; j++){
            cout << " ";
        }
        cout <<"*";
        if (i != 0){ 
          for(j = 0 ; j < 2 * i - 1; j++){ 
            cout << " ";
          }
          cout << "*";
        }
        cout <<"\n";
    }
    for(i = 0; i< column-1; i++){
        for(j  = 0; j <= i+1; j++){
            cout << " ";
        }
        cout << "*";
        if (i != (column-2)){ 
          for(j = 0 ; j < 2 * (column-i) - 5; j++){ 
            cout << " ";
          }
          cout << "*";
        }
        cout <<"\n";
    }
    return 0;
}
/* Butterfly pattern
   
   *               *
   * *           * *
   * * *       * * *
   * * * * * * * * *  
   * * * * * * * * *
   * * *       * * *
   * *           * *          
   *               *

*/
#include <iostream>
using namespace std;
int main(){
    int i,j,n;
    cout << "enter the value of n(n = row = column) : " << endl;
    cin >> n;
    for(i = 0; i<n; i++){
      for (j = 0; j<=i; j++){
        cout << "*";
      }
      for(j = 0; j < n -i-1; j++){
        cout << " ";
      }
      for(j = 0; j < n-i-1; j++){
        cout << " ";
      }
      for(j = 0; j<=i; j++ ){
        cout << "*";
      }
      cout << endl;
    }
    for(i = 0; i<n; i++){
      for (j = 0; j < n-i ; j++){
        cout << "*";
      }
      for(j = i; j>0; j--){
        cout << " ";
      }
      if(i != 0){
        for(j = 0; j<i; j++){
          cout << " ";
        }
      }
      for(j = 0; j < n-i ; j++ ){
        cout << "*";

      }
      cout << endl;
    }
    return 0;
}



