#include<iostream>
#include<string.h>
using namespace std;
int main() 
{
   cout<<"Welcome to encoder and decoder of Caesar Cipher!";
   int i, j, length,choice,key;
   cout<<"\nEnter the message to be worked upon: ";
   char msg[100], ch;
   cin.getline(msg,100); 
   cout << "Enter how many keys to be shifted: ";
   cin >> key; 
   length = strlen(msg);
   cout<<"Enter your choice \n1. Encryption \n2. Decryption \n";
   cin>>choice;
   switch(choice)
   {
      case 1:
      for(int i = 0; msg[i] != '\0'; ++i) 
      {
         ch = msg[i];
         if (ch >= 'a' && ch <= 'z')
         {
            ch = ch + key;
            if (ch > 'z') 
            {
               ch = ch - 'z' + 'a' - 1;
            }  
            msg[i] = ch;
         }
         else if (ch >= 'A' && ch <= 'Z')
         {
            ch = ch + key;
            if (ch > 'Z')
            {
               ch = ch - 'Z' + 'A' - 1;
            }
            msg[i] = ch;
         }
      }
      cout<<"Encrypted message: "<<msg;
      break;
      
      case 2:
      for(int i = 0; msg[i] != '\0'; ++i) 
      {
         ch = msg[i];
         if(ch >= 'a' && ch <= 'z') 
         {
            ch = ch - key;
            if(ch < 'a')
            {
               ch = ch + 'z' - 'a' + 1;
            }
            msg[i] = ch;
         }
         else if(ch >= 'A' && ch <= 'Z') 
         {
            ch = ch - key;
            if(ch < 'A') 
            {
               ch = ch + 'Z' - 'A' + 1;
            }
            msg[i] = ch;
         }
      }
      cout << "Decrypted message: " << msg;
      break;
   }
   return 0;
}
