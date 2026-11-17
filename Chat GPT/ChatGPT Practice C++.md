## فصل اول : ورودی، خروجی، عملیات ساده : 

**1- برنامه ای بنویسید که دو عدد به عنوان ورودی از کاربر دریافت کند و جمع و تفریق و ضرب و تقسیم را انجام دهد.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int a , b;
	cin >> a >> b;
	cout << a + b << endl; 
	cout << a - b << endl;
	cout << a * b << endl; 
	cout << a / b << endl;
	return 0;
}
```

**2- شعاع دایره را گرفته و محیط و مساحت آن را حساب کنید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	float r;
	cin >> r;
	cout << "Masahat :" << r * r * 3.14 << endl;
	cout << "Mohit :" <<r * 2 * 3.14 << endl;
	return 0;
}
```

**3- دما را به صورت سانتی گراد گرفته و به صورت فارنهایت نشان دهید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int degree;
	cin >> degree;
	cout << "The degree in F is:" << (degree * 1.8) + 32;
	return 0;
}
```

**4- سه عدد بگیرید و میانگین آن ها را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int a , b , c;
	cin >> a >> b >> c;
	cout << "The average is :" <<(a + b + c)/3;
	return 0;
}
```

**5- تعداد ثانیه را بگیرید و به دقیقه و ساعت و ثانیه تبدیل کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int s;
	cin >> s;
	int hour = s / 3600;
	int minute = (s % 3600) / 60;
	int second = (s % 3600) % 60;
	cout << hour << ':' << minute << ":" << second;
	return 0;
}
```

**6- مبلغی به تومان دریافت کرده و تعداد اسکناس های 10000 تومانی، 5000 تومانی و 1000 تومانی آن را حساب کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int price;
	cin >> price;
	int s10 = price / 10000;
	price = price % 10000;
	int s5 = price / 5000;
	price = price % 5000;
	int s1 = price / 1000;
	cout << "Number of 10000 is :" << s10 << endl;
	cout << "Number of 5000 is : " << s5 << endl;
	cout << "Number of 1000 is :" << s1 << endl;
	return 0;
}
```

**7- سرعت و زمان را بر اساس (km/h) دریافت کنید و مسافت طی شده را حساب کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int speed , hour;
	cin >> speed >> hour;
	int mile = speed * hour;
	cout << mile;
	return 0;
}
```

**8- طول و عرض یک مستطیل را گرفته و محیط و مساحت آن را حساب کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int x , y;
	cin >> x >> y;
	int masahat = x * y;
	int mohit = (2*x) + (2*y);
	cout << "The masahat is : " << masahat << endl;
	cout << "The mohit is :" << mohit << endl;
	return 0;
}
```

**9- یک عدد سه رقمی دریافت کرده و رقم یکان و دهگان و صد گان آن را نمایش دهید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	int number;
	cin >> number;
	int yekan = (number % 100) % 10;
	int dahgan = (number % 100) / 10;
	int sadgan = (number-(number % 100))/100;
	cout << "Yekan :" << yekan << endl;
	cout << "Dahgan :" << dahgan << endl;
	cout << "Sadgan :" << sadgan << endl;
	return 0;
}
```

**10- عددی بگیرید و مربع و مکعب آن را به دست آورید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	int number;
	cin >> number;
	cout << "Morabe :" << number * number << endl;
	cout << "Mokaab :" << number * number * number << endl;
	return 0;
}
```

## فصل دوم : شرط ها (if/else) : 

**1- عددی بگیرید و مشخص کنید مثبت، منفی یا صفر است.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int number;
	cin >> number;
	if (number > 0)
	{
		cout << "Positive";
	}
	else if (number < 0)
	{
		cout << "Negative";
	}
	else 
	{
		cout << "Your number is zero!";
	}
	return 0;
}
```

**2- عددی بگیرید و زوج یا فرد بودن آن را مشخص کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int number;
	cin >> number;
	if (number % 2 == 0)
	{
		cout << "Your number is even.";
	}	
	else if (number % 2 == 1)
	{
		cout << "Your number is odd.";
	}
	else 
	{
		cout << "Your number is Zero!";
	}
	return 0;
}
```

**3- دو عدد بگیرید و عدد بزرگ‌تر را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int number1;
	int number2;
	cin >> number1 >> number2;
	if (number1 > number2)
	{
		cout << "The bigger number is:" << number1;
	}
	else if (number1 < number2)
	{
		cout << "The bigger number is:" << number2;
	}
	else 
	{
		cout << "The number are equal!" << number1 << '=' << number2;
	}
	return 0;
}
```

**4- سه عدد بگیرید و عدد بزرگتر را مشخص کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int number1 , number2 , number3;
	cin >> number1 >> number2 >> number3;
	if (number1 > number2 && number1 > number3)
	{
		cout << "The biggest number is:" << number1;
	}
	else if (number2 > number1 && number2 > number3)
	{
		cout << "The biggest number is:" <<  number2;
	}
	else 
	{
		cout << "The biggest number is:" << number3;
	}
	return 0;
}
```

**5- سن فرد را بگیرید و اگر بیشتر از 18 سال داشت Adult نمایش داده شود در غیر این صورت Minor نمایش داده شود.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int age;
	cin >> age;
	if (age >= 18)
	{
		cout << "Adult";
	}
	else
	{
		cout << "Minor";
	}
	return 0;
}
```

**6- نمره دانشجویی را به عنوان ورودی دریافت کرده و اگر بالای 18 بود پیام عالی، بین 12 تا 18 بود پیام قبول و اگر زیر 12 بود مردود را نمایش دهید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	float score;
	cin >> score;
	if (score > 18)
	{
		cout << "Excellent";
	}
	else if (score >= 12 && score <= 18)
	{
		cout << "Pass";
	}
	else 
	{
		cout << "Fail";
	}
	return 0;
}
```

**7- عددی را به عنوان ورودی دریافت کرده و مشخص کنید که آیا بر 3 و 5 بخش پذیر است یا بخش پذیر نیست.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int number;
	cin >> number;
	if (number % 3 == 0 && number % 5 == 0)
	{
		cout << "Yes";
	}
	else 
	{
		cout << "No";
	}
	return 0;
}
```

**8-یک کاراکتر به عنوان ورودی بگیرید و مشخص کنید که حرف کوچک است یا بزرگ.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	char myChar;
	cin >> myChar;
	if (int(myChar) >= 65 && int(myChar) <= 90)
	{
		cout << "Your Character is in Big Case!" << myChar;
	}
	else if (int(myChar) >= 97 && int(myChar) <= 122)
	{
		cout << "Your Character is in Small Case!" << myChar;
	}
	else 
	{
		cout << "Invalid Character!";
	}
	return 0;
}
```

**9- قیمت کالا را به عنوان ورودی دریافت کرده و اگر بالای یک میلیون بود شامل ده درصد تخفیف می شود. مبلغ نهایی را به کاربر نمایش دهید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int price;
	cin >> price;
	if (price >= 1000000)
	{
		price = price - ((price * 10)/100);
		cout << "You should pay :" << price << "After 10%.";
	}
	else
	{
		cout << "You should pay:" << price;
	}
	return 0;
}
```

**10- معادله درجه دو را بر اساس دلتا بگویید، چند جواب دارد.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	int delta;
	cin >> delta;
	if (delta < 0)
	{
		cout << "Your Equation doesn't have answer!";
	}
	else if (delta == 0)
	{
		cout << "Your Equation has 2 reapeted answer!";
	}
	else 
	{
		cout << "Your Equation has 2 diffrent real answer!";
	}
	return 0;
}
```


## فصل سوم : حلقه های for و while : 

**1- عدد n را به عنوان ورودی بگیرید و اعداد 1 تا n را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for (int i = 0 ; i <= n ; i++)
    {
        cout << i;
    }
    return 0;
}
```

**2- عدد n را به عنوان ورودی بگیرید و مجموع اعداد 1 تا n را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    int sum = 0;
    cin >> n;
    for (int i = 0 ; i <= n ; i++)
    {
        sum += i;
    }
    cout << sum;
    return 0;
}
```

**3- جدول ضرب یک عدد را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for (int i = n ; i == n ; i++)
    {   
        for (int j = 1; j <= 10 ; j++)
        {
            cout << i * j;
            cout << endl;
        }
	}
	return 0;
}
```

**4- فاکتوریل یک عدد را حساب کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int number;
    cin >> number;
    int factorial = 1;
    for (int i = 1 ; i <= number ; i++)
    {
        factorial *= i;
    }
    cout << factorial;
    return 0;
}

```

**5- عددی را به عنوان ورودی دریافت کرده و تعداد رقم های آن را حدس بزنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    int count = 0;
    cin >> n;
    while (n != 0)
    {
        n = n / 10;
        count += 1;
    }
    cout << count;
    return 0;
}
```

**6- عددی را به عنوان ورودی دریافت کرده و برعکس آن را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int number;
    int digit = 0;
    int reversenumber = 0;
    cin >> number;
    while (number != 0)
    {
        digit = number % 10;
        reversenumber = reversenumber * 10 + digit ;
        number = number / 10;
    }
    cout << reversenumber;
    return 0;
}
```

**7- عددی را به عنوان ورودی دریافت کرده و مجموع ارقام آن را حساب کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int number;
    int digit = 0;
    int sumnumber = 0;
    cin >> number;
    while (number != 0)
    {
        digit = number % 10;
        sumnumber = sumnumber + digit ;
        number = number / 10;
    }
    cout << sumnumber;
    return 0;
}
```

**8- عددی را به عنوان ورودی دریافت کرده و تمامی مقسوم علیه های آن را چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int number;
    cin >> number;
    for (int i = 1 ; i <= number ; i++)
    {
        if(number % i == 0)
        {
            cout << i << endl;
        }
        else 
        {
            
        }
    }
    return 0;
}
```

**9- عددی را به عنوان ورودی دریافت کرده و مشخص که این عدد اول است یا نه.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int number;
    int count = 0;
    cin >> number;
    for (int i = 1 ; i <= number ; i++)
    {
        if(number % i == 0)
        {
            count += 1;
        }
        else 
        {
            
        }
    }
    if (count == 2)
    {
        cout << "Number is Aval";
    }
    else 
    {
        cout << "Number isn't Aval";
    }
    return 0;
}
```

**10- دو عدد به عنوان ورودی دریافت کرده و بزرگترین مقسوم علیه مشترک دو عدد را پیدا کنید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
    int number1;
    int number2;
    int bmm;
    cin >> number1 >> number2;
    while (number2 != 0)
    {
        bmm = number1 % number2;
        number1 = number2;
        number2 = bmm;
    }
    cout << number1;
    return 0;
}
```

## فصل چهارم : حلقه های تو در تو : 

**1- یک عدد دریافت کرده و به ازای آن یک مربع n×n چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main ()
{
    int n;
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        for (int j = 0 ; j < n; j++)
        {
            cout << "*";
        }
    cout << endl;
    }
    return 0;
}
Output:
in : 4
****
****
****
****
```

**2-دو عدد به عنوان row و column دریافت کنید و سپس مستطیلی با * چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main ()
{
    int row , column;
    cin >> row >> column;
    for (int i = 0; i < row; i++)
    {
        for (int j = 0 ; j < column; j++)
        {
            cout << "*";
        }
    cout << endl;
    }
    return 0;
}
Output:
in : 3 4
****
****
****
```

**3- جدول ضرب 10 در 10 بنویسید.** 

```C++
#include <iostream>
using namespace std;
int main ()
{
    for (int i = 1; i <= 10; i++)
    {
        for (int j = 1 ; j <= 10; j++)
        {
            cout << i * j  << " ";
        }
    cout << endl;
    }
    return 0;
}
Output:
1 2 3 4 5 6 7 8 9 10 
2 4 6 8 10 12 14 16 18 20 
3 6 9 12 15 18 21 24 27 30 
4 8 12 16 20 24 28 32 36 40 
5 10 15 20 25 30 35 40 45 50 
6 12 18 24 30 36 42 48 54 60 
7 14 21 28 35 42 49 56 63 70 
8 16 24 32 40 48 56 64 72 80 
9 18 27 36 45 54 63 72 81 90 
10 20 30 40 50 60 70 80 90 100 
```

**4- یک عدد n دریافت کنید و مثلثی از 1 تا n رسم کنید.** 

```C++
#include <iostream>
using namespace std;
int main()
{
	int n;
	cin >> n;
	for (int i = 1; i <= n; i++)
	{
		for (int j = 1; j <= i; j++)
		{
			cout << "*";
		}
	cout <<endl;
	}
	return 0;
}
Output: 
in : 4 
*
**
***
****
```

**5- یک عدد n دریافت کنید و از n تا 1 مثلث کاهشی رسم کنید.**

```C++
#include <iostream>
using namespace std;
int main ()
{
    int n;
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = i ; j <= n; j++)
        {
            cout << "*" ;
        }
        cout << endl;
    }
    return 0;
}
Output:
in : 4 
****
***
**
*
```

**6- یک عدد n به عنوان ورودی دریافت کرده و از 1 تا اعداد قبل از آن را به ترتیب و در خط های جدا چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main ()
{
    int n;
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1 ; j <= i; j++)
        {
            cout << j ;
        }
        cout << endl;
    }
    return 0;
}
Output:
5
1
12
123
1234
12345
```

**7- عدد n را به عنوان ورودی از کاربر دریافت کرده و و سپس اعداد را از 1 تا n به اندازه شماره ردیف چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main ()
{
    int n;
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1 ; j <= i; j++)
        {
            cout << i ;
        }
        cout << endl;
    }
    return 0;
}
Output:
1
22
333
4444
55555
```

**8- عدد n را به عنوان ورودی دریافت کرده و مربعی تو خالی با ابعاد n×n رسم کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for (int i = 1; i <= n ; i++)
    {
        for (int j = 1 ; j <= n; j++)
        {
            if ((i == 1 || i == n) || (j == 1 || j == n))
            {
                cout << "*";
            }
            else
            {
                cout << " ";
            }
        }
    cout << endl;
    }
    return 0;
}
Output:
in : 4
****
*  *
*  *
****
```

**9- عدد n را به عنوان ورودی دریافت کرده و با آن هرم ستاره ای چاپ کنید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int n;
	cin >> n;
	for (int i = 1; i <= n; i++)
	{
		for (int j = 1; j <= n - i; j++)
		{
            cout << " ";
		}
		for (int j = 1; j <= 2 * i - 1; j++)
		{
		    cout << "*";
		}
		cout << endl;
	}
	return 0;
}
Output:
in : 4
   *
  ***
 *****
*******
```

**10- عدد n را به عنوان ورودی دریافت کرده و n×n جدول مختصات بسازید.**

```C++
#include <iostream>
using namespace std;
int main()
{
	int n;
	cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
        {
            cout << "(" << i << "," << j << ")" << " "; 
        }
        cout << endl;
    }
    return 0;
}
Output:
in : 4
(1,1) (1,2) (1,3) (1,4) 
(2,1) (2,2) (2,3) (2,4) 
(3,1) (3,2) (3,3) (3,4) 
(4,1) (4,2) (4,3) (4,4) 
```

## فصل پنجم : تابع : 

