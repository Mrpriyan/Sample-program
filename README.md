# Sample-program 1
# competitive easy programming question
#include <iostream>
using namespace std;
void disp( char a,int j)
{
    int b=j-48;
    for(int i=0;i<b;i++)
    {
        cout<<a;
    }
}

int main() {
   string a;
   cout<<"Enter the string:";
   cin>>a;
   int l=a.length();
   for(int i=0;i<l;i+=2)
 {
  disp(a[i],a[i+1]);  
 }
    return 0;
}
# OUTPUT
Enter the string:S4G7
SSSSGGGGGGG


# Sample-program 2
# Program to reverse vowels in a given string
#include <iostream>
using namespace std;
bool isvowel(char x)
{
  if (x == 'a' || x == 'e' || x == 'i' || x == 'o'
        || x == 'u' || x == 'A' || x == 'E' || x == 'I'
        || x == 'O' || x == 'U')
    return true;
    else
        return false;
}
int main()
{
string a;
cout<<"Enter the string:";
cin>>a;
int l=a.length();
for(int i=0;i<l;i++)
{
 for(int j=i+1;j<l;j++)
 {
     if(isvowel(a[i]) && isvowel(a[j]))
     {
         if(a[i]<a[j]) swap(a[i],a[j]);
     }
 }
}
cout<<a;
return 0;
}
# OUTPUT
Enter the string:abcdef
ebcdaf
