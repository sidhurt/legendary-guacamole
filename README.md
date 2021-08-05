# legendary-guacamole
 Write a program to calculate total volume of different measure (shapes) such as cube, sphere, cylinder and cone. Write separate functions as inline functions for each shape and return their volume to main for total calculation. Display total volume in main function.

#include <iostream>
using namespace std;
float PI=3.14;
float vol(int);
float vol(float);
float vol(float, int);
float vol(int, int);


inline float vol (int a)
{
int v;
v= a*a*a;
return v;
}
inline float vol (float r)
{
float v;
v=(4/3)*PI*r*r*r;
return v;
}
inline float vol (int b, int c)
{
float v;
v=PI*b*b*c;
return v;
}
inline float vol (float d, float e)
{
float v;
v=(PI*d*d*e)/3;
return v;
}
int main()
{
int a;
cout<<"enter the value of side of a"<<endl;
cin>>a;
cout<<"the vol of cube is "<< vol(a)<<endl;
float r;
cout<<"enter the value of sphere"<<endl;
cin>>r;
cout<<"the volume the sphere is "<<vol(r)<<endl;
int b,c;
cout<<"enter the measures of radius and height of a cylinder"<<endl;
cin>>b>>c;
cout<<"the volume of the cylinder is "<<vol(b,c)<<endl;

float d,e;
cout<<"enter the measures of radius and height of a cone"<<endl;
cin>>d>>e;
cout<<"the volume of the cone is "<<vol(d,e)<<endl;
}
