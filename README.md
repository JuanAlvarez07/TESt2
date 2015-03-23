#include <iostream>
using namespace std;

double baby (double n){
  double error= .0001;
  double s=n;

  while((s - (n/s)) > error){
    s=(s+ n/s)/2;
    cout<<s<<endl;
  }
  return s;
}

int main(){

  double number=125348;
  double result = baby(number);

  cout<<"Baby: "<<result<<endl;
  return 0;


