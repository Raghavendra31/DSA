#include<iostream>
#include<string>
using namespace std;
int main()
{
   string  ragu {"abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ "};
   string  aaaa {"!1@#3$4%5^&7*_-+={[}]:'<,>.?/}ßΓπΣσµτΦΘδ∞φε∩≡±≥≤3⌡≈°⌠"};
   string msg;
   string encryption;
   string decryption;

   cout<<"enter your msg:";
   getline(cin,msg);

   cout<<endl<<"your msg is encrypting......"<<endl;
   for(char r:msg)
   {
      int position=ragu.find(r);   // size_t is to find the char position...
      if(position != string::npos)    //npos means no results found kind of stuff...  npos = -1;
      {
         char new_r=aaaa.at(position);
         encryption += new_r;
      }
      else
      {
         encryption += r;
      }
   }
   cout<<endl<<"encrypted msg is:"<<encryption<<endl;

   cout<<endl<<"your msg is decrypting....."<<endl;
   
   for(char b:encryption)
   {
       int ra=aaaa.find(b);
       if(ra != string::npos)
       {
         char gu = ragu.at(ra);
         decryption += gu;

       }
       else{
         decryption += b;
       }
       
   }
   cout<<endl<<"decrypted msg is : "<<decryption<<endl;
   return 0;
};
