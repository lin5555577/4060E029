# 4060E029

###### exercise1 矩陣相加 2018/4/17

```
#include <stdio.h>
int main(void)
{
int i,j;
int a[3][3],b[3][3],c[3][3];
printf("please input the array for a:\n"); 
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
scanf("%d",&a[i][j]);
}
}
printf("please input the array for b:\n"); 
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
scanf("%d",&b[i][j]);
}
}
printf("now the array c is :\n");
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
c[i][j] = a[i][j]+b[i][j];
printf("%5d",c[i][j]);
}
printf("\n");
}
return 0;
}

```

###### exercise2 矩陣相乘 2018/4/17

```
#include <stdio.h>
int main(void)
{
int i,j;
int a[3][3],b[3][3],c[3][3];
printf("please input the array for a:\n");
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
scanf("%d",&a[i][j]);
}
}
printf("please input the array for b:\n"); 
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
scanf("%d",&b[i][j]);
}
}
printf("now the array c is :\n"); 
for(i = 0; i < 3; i++)
{
for(j = 0; j < 3; j++)
{
c[i][j] = a[i][j]*b[i][j];
printf("%5d",c[i][j]);
}
printf("\n");
}
return 0;
}


```
###### exercise3

```
#include <iostream>
using namespace std;
int main()
{
	int i,a[10];

	for(i=0;i<10;i++)
		a[i]=i;

	for(i=0;i<10;i++)
		cout << a[i] << endl;
		
			cout << "4060E029 2018.04.17" << endl;
    return 0;
}


```



###### exercise4
```
// C++ program to demonstrate various function string class
#include <bits/stdc++.h> //使用標準c++標頭檔
using namespace std;  //使用名稱空間

int main()
{
	// various constructor建構子 of string class不同的建構子

	// initialization by raw string //宣告字串str1
	string str1("first string");

	// initialization by another string//使用字串物件
	string str2(str1);

	// initialization by character with number of occurence //宣告字串str3 產生5個#
	string str3(5, '#');

	// initialization by part of another string
	string str4(str1, 6, 4); // from 6th index (second parameter)
							// 6 characters (third parameter)

	// initialization by part of another string : iteartor version
	string str5(str2.begin(), str2.begin() + 5);

	cout << str1 << endl;  //會輸出 first string
	cout << str2 << endl;  // 會輸出 first string
	cout << str3 << endl;  // 會輸出 #####
	cout << str4 << endl;
	cout << str5 << endl;

	// assignment operator
	string str6 = str4;

	// clear function deletes all character from string
	str4.clear();

	// both size() and length() return length of string and
	// they work as synonyms
	int len = str6.length(); // Same as "len = str6.size();"

	cout << "Length of string is : " << len << endl;

	// a particular character can be accessed using at /
	// [] operator
	char ch = str6.at(2); // Same as "ch = str6[2];"


	cout << "third character of string is : " << ch << endl;

	// front return first character and back returns last charcter
	// of string

	char ch_f = str6.front(); // Same as "ch_f = str6[0];"
	char ch_b = str6.back(); // Same as below
							// "ch_b = str6[str6.length() - 1];"

	cout << "First char is : " << ch_f << ", Last char is : "
		<< ch_b << endl;

	// c_str returns null terminated char array version of string
	const char* charstr = str6.c_str();
	printf("%s\n", charstr);

	// append add the argument string at the end
	str6.append(" extension");
	// same as str6 += " extension"

	// another version of appends, which appends part of other
	// string
	str4.append(str6, 0, 6); // at 0th position 6 character

	cout << str6 << endl;
	cout << str4 << endl;

	// find returns index where pattern is found.
	// If pattern is not there it returns predefined
	// constant npos whose value is -1

	if (str6.find(str4) != string::npos)
		cout << "str4 found in str6 at " << str6.find(str4)
			<< " pos" << endl;
	else
		cout << "str4 not found in str6" << endl;

	// substr(a, b) function returns a substring of b length
	// starting from index a
	cout << str6.substr(7, 3) << endl;

	// if second argument is not passed, string till end is
	// taken as substring
	cout << str6.substr(7) << endl;

	// erase(a, b) deletes b character at index a
	str6.erase(7, 4);
	cout << str6 << endl;

	// iterator version of erase
	str6.erase(str6.begin() + 5, str6.end() - 3);
	cout << str6 << endl;

	str6 = "This is a examples";

	// replace(a, b, str) replaces b character from a index by str
	str6.replace(2, 7, "ese are test");

	cout << str6 << endl;

	return 0;
}







```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
###### exercise4
```

```
