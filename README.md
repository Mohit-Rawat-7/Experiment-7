# AIM 
To create array in c++ and doing basic operations on it.

# Software Used
VS Code

# Problem Statement

1.) Write a c++ code to make an array.

2.) Write a c++ code to make an array with elements in reverse order in which user entered.

3.) Write a c++ code to make do sum and average of array elements.

4.) Write a c++ code to find maximum and minimum element of an array.

5.) Write a c++ code to search the position of element, number of time it is occuring in an array.
 
 6.) Write a c++ program to take input from user. 

 7.) Write a c++ program to concatenate the string on c++. 

 8.)  Write a c++ program to reverse string. 

 9.)  Write a c++ program to check a palindrome.


# Theory
In C++, an array is a data structure that is used to store multiple values of similar data types in a contiguous memory location.

 C++ strings are sequences of characters stored in a char array. Strings are used to store words and text. They are also used to store data, such as numbers and other types of information. Strings in C++ can be defined either using the std::string class or the C-style character arrays.

# Program Codes

```javascript
//Array
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements";
    cin >> n;
    int a[n];
    cout << " Enter array elements";
    for ( int i =0; i <n ; i++ )
    { cin >> a[i];
     
    }
       for (int i: a)
     {
        cout << " "<< i ;
     } 
    return 0;
}

//Reverse array
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements";
    cin >> n;
    int a[n];
    cout << " Enter array elements";
    for ( int i =0; i <n ; i++ )
    { cin >> a[i];
     
    }
       for (j = n-1 ; j>=0; j--)
     {
        cout << " "<< a[j];
     } 
    return 0;
}

//Sum & average of array elements
#include<iostream>
using namespace std;
int main()
{
     int n, i, j;
     float avg, s = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}

for (j= 0 ; j<n; j++)
{
    s = a[j]+s;
}
avg = s/n;
cout << "The sum of elements of the givne array is: "<<s<<endl;
cout << "The average of the given array is: "<< avg<<endl;

return 0;
}

//Maximum and minimum
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, max, min;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
max = a[0];
min = a[0];
for (j= 1 ; j<n; j++)
{
 if (max<a[j])

 {
    max = a [j];
 }
 if (min > a[j])
 {
    min = a[j];
 }
}
cout <<"The maximum element in the given array is: "<<max<<endl;
cout << " The minimun element in the array is: "<<min<<endl;
return 0;

}

//Search element
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, s, c = 0, flag = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
cout << "Enter an element to be searched in an array: ";
    cin >> s;
for (j= 0 ; j<n; j++)
{
    if ( a[j]==s)
    {
cout<< "The element"<<" "<< s<< " " << "is present at location: "<<j<<endl;
c++;
flag =1;
    }
}

if( flag ==0)
{
    cout<< "The element"<< " "<< s << " "<< "is not present in the given array";
}
else
{
    cout << "The element" << " "<< s << " "<< "occurs"<< " "<< c << " "<< "times.";
}
return 0;
}
//USER INPUT
#include <iostream>
using namespace std;
int main()
{
    char s[]= "Mohit";
    cout<<s<<endl;
    return 0;
}


//CONCATENATION
#include<iostream>
using namespace std;
int main() 
{
    string name("Mohit");
    string surname("Rawat");
    name.append(surname);
    cout<<name<<endl;
}


//REVERSE STRING
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main()
{
string a= "Mohit";
reverse(a.begin(), a.end());
cout<<"reverse string is:"<<a<<endl;
return 0;
}

//PALINDROME
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main() 
{
    string s1, s2;
    cout << "Enter a word to check";
    cin>>s1;
    s2=s1;
    reverse(s1.begin(), s1.end());
    if (s2==s1) 
    {
        cout<<"Yes! It is a palindrome";
    }
    else cout<<"No! It is not a palindrome";
}

```
# Output
1.)
![image](https://github.com/user-attachments/assets/1c9d4f35-9433-4bbe-9c7a-0fc7892ac819)

2.)
![image](https://github.com/user-attachments/assets/ca699330-e0de-470a-aa3d-76d87a8428c0)

3.)
![image](https://github.com/user-attachments/assets/4bde05ef-54eb-4b8a-900f-e905987ab0ca)

4.)
![image](https://github.com/user-attachments/assets/f2f4df6a-1cb8-43b0-b02f-bc9283124f5f)

5.)
![image](https://github.com/user-attachments/assets/f0a593e1-229c-4469-8638-dceb61ad64ae)

6.)
![image](https://github.com/user-attachments/assets/937d63f5-05b9-467c-aa04-c0037711d2f8)

7.)
![image](https://github.com/user-attachments/assets/87745879-9995-4a5d-8a9d-f879352b930d)

8.)
![image](https://github.com/user-attachments/assets/7169c3e3-2955-4752-b1bd-2e9b4a556638)

9.)
![image](https://github.com/user-attachments/assets/9ed1a243-02fa-4cc5-a069-b14bc8a1872c)


# Conclusion

We learnt to create an array and operate it. 

We learnt to search element in the array and getting the sum and average of the elements.

We learnt to do concatenation of strings, making and checking palindromes, reversing the string in c++..
