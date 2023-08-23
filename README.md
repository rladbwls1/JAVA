# 연산자 (Operations)
### 연산이란?
* 데이터를 처리하여 결과를 산출하는 것
연산자의 종류
![image](https://github.com/rladbwls1/JAVA/assets/105581525/6e147b02-c0ac-4e82-b00f-dc2b1730008c)


증감연산자
```
class OperEx01 
{
	public static void main(String[] args) 
	{
		int a = 10;
		System.out.println(++a);	// 11
	}
}
```

```
class OperEx01 
{
	public static void main(String[] args) 
	{
		int a = 10;
		System.out.println(a++);	// 10
		System.out.println(a);		// 11
	}
}
```

```
class OperEx01 
{
	public static void main(String[] args) 
	{
		int a = 10;
		System.out.println(++a);	// 11
		System.out.println(a++);	// 11	(12)
		System.out.println(++a);	// 13
		System.out.println(++a);	// 14
		System.out.println(a++);	// 14	(15)
		System.out.println(++a);	// 16
		System.out.println(a);	// 16
	}
}
```
### 산술 연산자
![image](https://github.com/rladbwls1/JAVA/assets/105581525/8d10a56b-e227-4115-897a-13c665186b9b)
```
class OperEx02 
{
	public static void main(String[] args) 
	{
		// byte -128 ~ 127
		byte a = (byte)(100 + 30);	// 오버플로우 발생
		System.out.println(a);
	}
}
```
오버플로우 : 메모리의 표현 범위에서 벗어난 수의 값을 저장하는 경우

