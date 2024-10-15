#include<bits/stdc++.h>
using namespace std;
void rev(char *arr,int n)
{
  char *end=arr;
  while(*end)
  {
    end++;
  }
  end--;
  while(end>arr)
  {
    char temp=*arr;
    *arr=*end;
    *end=temp;
  }
  cout<<arr;
}
int main() {
  char arr[]="helloworld";
  int n=sizeof(arr)/sizeof(arr[0]);
  rev(arr,n);    
  return 0;
}
