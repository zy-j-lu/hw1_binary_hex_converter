# hw1_binary_hex_converter
#include <iostream>
#include <string>
using namespace std;
  
int main()  
{  
  int store[9], n, p, num, j, i;
  char arr[16] = {'0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F'};
  char hex[16];

  cout<<"請輸入欲轉換的數字(0-255)：";    
  cin>>n;
  num=n;

  for(p=0; n>0; p++)
  {
    store[p]=n%2;
    n= n/2;
  }
  cout<<"此數字的二進位是：";
  for(p=p-1 ;p>=0 ;p--)
  {
    cout<<store[p];
  } 
  cout << "\n";
  
  for(i=0; num>0; i++)
  {
      hex[i] = arr[num % 16];
      num = num / 16;
  }
  cout<<"此數字的16進位是：";
  for (j = i - 1; j >= 0; j--)
  {
      cout<<hex[j];
  }
  return 0;
}
