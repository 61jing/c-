# c-
某些习题的相关程序，包括自己写的和对书上的注释记录。
7.
#include<iostream>
using namespace std;
int main()//主函数，实现功能输出c
	{
		int a,b,c;
		int f(int x,int y,int z);
		cin>>a>>b>>c;
		c=f(a,b,c);//c由函数f决定
		cout<<c<<endl;
		return 0;
}
int f(int x,int y,int z)//定义函数f的功能
{//通过比较实现找出最小值
	int m;
	if(x<y)m=x;
	else m=y;
	if(z<m)m=z;
	return(m);

}

8. #include<iostream>
using namespace std;
int main()
{
int a,b,c;
cin>>a>>b;
c=a+b;
cout<<"a+b="<<c<<endl;
return 0;

}

9./*定义add函数进行相加并且输出*/
#include<iostream>
using namespace std;
int main()
{
   int a,b,c;
   cin>>a>>b;
   int add(int x,int y);
   c=add(a,b);
   cout<<"a+b="<<c<<endl;
   return 0;
}
int add(int x,int y)
{
	int z;
	z=x+y;
	return z;
}


10./*从小到大输出三个数*/
#include<iostream>
using namespace std;
int main()
{
	void sort(int x,int y,int z);
	int x,y,z;
	cin>>x>>y>>z;
	sort(x,y,z);
	return 0;
}
void sort(int x,int y,int z)
{
	int temp;
	if(x>y){temp=x;x=y;y=temp;}//else x,y,—>z和y比较后直接输出
	if(z<x) cout<<z<<','<<x<<','<<y<<endl;
	else if(z<y) cout<<x<<','<<z<<','<<y<<endl;
	else cout<<x<<','<<y<<','<<z<<endl;
}
