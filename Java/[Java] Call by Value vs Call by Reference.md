## Call by value ve Call by Reference

간단하면서도 헷갈리는 개념 중 하나이다. 

결론은 자바는 `Call by Value`이다.



Primitive Type(원시 자료형)의 경우 Call by Value

- int, short, long, float, double, char, boolean



Reference Type(참조 타입)의 경우 Call by Value

- Array, 참조 타입



자바에서는 함수의 인자로 전달되는 타입이 기본형(원시 자료형)인 경우 값을 넘기게 되어있다. 이 경우 메모리 공간에서는 함수를 위한 별도의 공간이 생성된다. 이는 함수 종료시 사라진다. 따라서 함수 안에서 해당 인자의 값을 변경하더라도 원본 값은 바뀌지 않는 특징이 있다.

참조형(참조 타입)인 경우, 변수가 가지는 값이 주소 값이므로 Call by Value에 의해 주소 값이 전달된다. 따라서 함수 안에서 해당 인자의 값을 변경하게 되면 원본 값도 바뀌게 되는 특징이 있다.