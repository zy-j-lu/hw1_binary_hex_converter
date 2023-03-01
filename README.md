# hw1_binary_hex_converter

#include <iostream>
#include <string>
using namespace std;
  
int main()  
{  
  int store[9], n, p;
  int i, j, num, a = 0;
  char arr[16] = "'0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F'";
  char hex[16];
  a = num;
  cout<<"請輸入欲轉換的數字(0-255)：";    
  cin>>n;
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
  
  while (num)
  {
      hex[i++] = arr[num % 16];
      num = num / 16;
  }
  cout<<"此數字的16進位是：";
  for (j = i - 1; j >= 0; j--)
  {
      cout<< arr[j]);
  ]
  return 0;
}
