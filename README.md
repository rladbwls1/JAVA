# 연산자 (Operations)
### 연산이란?
* 데이터를 처리하여 결과를 산출하는 것
연산자의 종류
![image](https://github.com/rladbwls1/JAVA/assets/105581525/6e147b02-c0ac-4e82-b00f-dc2b1730008c)
</br></br>
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
**++a** : 증감연산자 먼저 실행하므로 값 11
 <br/><br/>
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
**a++** : 증감연산자 마지막으로 실행하므로 값 10 (그 다음 a 출력시 값 11)
 <br/><br/><br/>
**증감연산자 예시**
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
<br/><br/>
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
**오버플로우** : 메모리의 표현 범위에서 벗어난 수의 값을 저장하는 경우
<br/><br/>

### 비교 연산자
* 대소 또는 동등 비교해서 boolean 타입인 true/false 산출
![image](https://github.com/rladbwls1/JAVA/assets/105581525/d583266d-044a-46be-a68d-30dfc5e9866b)

```
class OperEx03  
{
	public static void main(String[] args) 
	{
		int a = 10;
		int b = 5;
		System.out.println(a > b);	//T
		System.out.println(a < b);	//F
		System.out.println(a >= b);	//T
		System.out.println(a <= b);	//F
		System.out.println(a == b);	//F
		System.out.println(a != b);	//T

	}
}
```
<br/><br/>

### 논리 연산자
* 논리곱, 논리합, 배타적 논리합, 논리 부정 연산 수행
* 피연산자는 boolean 타입만 사용 가능!
![image](https://github.com/rladbwls1/JAVA/assets/105581525/fe404966-17c5-4026-b1fc-db4dce0aa8ec)
<br/>
* 논리연산자 예시
  
```
class OperEx04 
{
	public static void main(String[] args) 
	{
		int a = 10;
		boolean r = a > 0 && a > 5 && a > 10;
		System.out.println(r);	// false

		r = a > 0 || a > 5 || a > 10;
		System.out.println(r);	// true

		boolean result = true;
		System.out.println(!result);	// ! 부정문 false

		result = a > 0 ^ a > 5;
		System.out.println(result);	// false
	}
}
```
**- a > 0 : True**<br/>
**- a > 5 : True**<br/>
**- a > 10 : False**<br/>
<br/><br/>

### 진법
**2진수 : 0, 1**<br/>
**8진수 : 0 ~ 7**<br/>
**10진수 : 0 ~ 9**<br/>
**16진수 : 0 ~ 15**<br/>
