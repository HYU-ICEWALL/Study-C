# Day1: 변수와 함수
아래는 우리가 프로그램을 작성하는데 있어서 필요한 몇가지 준비물 입니다.

이제 하나하나 살펴보기 전에 C에 대한 기본적인 지식을 훑어봐요.
C 코드는 마치 레시피 같아요.
레시피에서 재료와 조리방법들이 적혀있듯, C 코드도 그러한 것들을 필요로해요.

오늘은 C언어의 **변수**, **함수**를 배울거에요.

-----

## 변수
변수는 레시피의 재료와 비슷해요. 
C코드 내부에서 미리 준비해야하고, 변경될 수 있으며 결과물에 반영이되죠.

재료들이 종류에 따라 다루는 방법이 다르듯 C에서도 변수는 종류에 따라 다루는 방법이 달라요.
이러한 종류를 '자료형'이라 불러요. 수 많은 자료형이 있지만 대표적으로 아래 세개를 먼저 배울게요.

- int
- float
- char

**int**는 정수 자료형이에요. **float**은 실수를 담을 수 있고, **char**은 문자를 담을 수 있어요.
이러한 자료형은 보통 메모리 공간에서의 크기로 구별지어져요. 하지만 이런 이야기는 조금 어려우니 후술할게요.

>[variable.c](https://github.com/MaybeS/STUDY2016/blob/master/Day1/example/variable.c)

위의 예제에서 변수를 선언하고 다루는 간단한 방법들을 읽힐 수 있어요.

## 함수
요리책 전체에걸쳐 이런 저런 방법으로 손질한 감자가 계속 쓰인다면, 이 재료를 따로 표시해서 방법을 매번 적지 않고
'손질한 감자'를 준비하세요.라고 할수도 있겠죠. 바로 이러한 기능을 하는것이 함수에요.

C에서의 함수는 기본적으로 아래와 같이 생겼어요.
```
[return type] [function_name]([arg_type] [arg_name], ...)
{
	/* codes */
}
```
>[function.c](https://github.com/MaybeS/STUDY2016/blob/master/Day1/example/function.c)

return type과 arg type은 둘다 위에서 언급한 변수의 자료형이 들어가요.
function name은 함수의 이름을 쓰고, arg name은 변수의 이름을 써요.

함수의 이름을 제외한 다른 모든 것은 생략될 수 있어요.

즉 아주 간단하게 함수를 만들면

```
void this_is_function() 
{
	/* codes */
}
```
이것도 함수가 될 수 있어요. void는 함수의 반환자가 없다는 표시를 나타내요. (즉 값을 돌려주지 않을꺼라는거죠)

위에서 언급한 것 처럼 어떤 변수에 5를 곱하고 3을 더하고 2를 빼는 작업을 여러번 해야 한다면 함수로 만들 수 있겠죠.
한번 도전해보세요.

**Day2에서 만나요**