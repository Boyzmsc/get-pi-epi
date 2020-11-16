# PI/EPI 찾기 프로그램



**이 프로젝트는 국민대학교 논리회로설계 강의를 바탕으로 제작되었습니다.**

C++ 프로그래밍 언어를 이용해 제작했으며,
비트 수를 입력하고 그에 따라 입력받는 minterm과 don't care에 따른 Prime Implicants와 Essential Prime Implicants를 구하는 프로그램이다.

------



## 목차

|   내용    |
| :-------: |
| 실행 방법 |
| 소스 코드 |





## 실행 방법

1) 소스 파일을 컴파일 한 뒤 실행합니다.

2) 비트 수를 입력합니다.

* 0 이하의 수는 받지 않습니다.

3) minterm을 입력합니다.

* -1을 입력 시 입력이 종료되며, 음수나 반복된 수는 받지 않습니다.

4) don't care를 입력합니다.

* -1을 입력 시 입력이 종료되며, 음수나 반복된 수는 받지 않습니다. minterm에 포함된 수도 받지 않습니다.

5) 결과가 출력됩니다.

* Minterm : 입력한 minterm을 출력합니다.

* Don't care : 입력한 don't care을 출력합니다.

* Binary List : minterm과 don't care의 비트 수에 따른 이진 데이터를 출력합니다.

* Prime Implicants : PI를 출력합니다.

* One repeat Minterm : minterm과 don't care중에서 한번만 나오는 요소들을 출력합니다.

* Final One repeat Minterm : don't care을 제외한 한번만 나오는 minterm들을 출력합니다.

* Essential Prime Implicants : EPI를 출력합니다.

6) 출력 화면

![screenshot](https://user-images.githubusercontent.com/28584213/99257128-de32be80-2859-11eb-8aa8-2d6cf48b974d.png)






## 소스 코드

* binaryToNum
  * 2진수의 형태를 10진수로 바꾸는 함수

* getPossibleElements
  * PI가 표현할 수 있는 minterm들을 담는 vector 리턴
* getPossible
  * getPossibleElements 메서드로 나오는 vector들을 결합

* isEqual
  * 두 vector가 같은지 판단 (phaseUP 메서드 동작 판단)
* checkInVectorString
  * string이 vertor에 있는지 확인
* checkInVectorInt
  * int가 vector에 있는지 확인

* getCompareBinary
  * 0001 , 0011 -> 00-1 처럼 변환하는 함수
* isCompareBinary
  * 0001, 0011 처럼 두 이진수가 한끗 차이 나느냐 판단
* getBinary
  * 10진수를 2진수로 전환하는 함수
* getBinaryList
  * int형 vector을 string형 vector로 바꿈
* phaseUp
  * 한끗 차이 나는 것끼리 묶어 다음 단계로 이동, 포함 안된 것들도 같이 포함
* printList
  * vertor내 요소들 출력
* getFrequencyOf
  * 해당 인수의 빈도수 반환
* getOneRepeatNum
  * EPI에 해당하는 minterm이 담긴 vector 반환
* getIndexOf
  * 해당 원소의 index 반환
* minusDontCare
  * EPI에 해당하는 minterm에서 don't care minterm을 뺌
* isEpi
  * PI가 EPI인지 확인
  * PI가 나타낼 수 있는 minterm중에 final one repeat minterm에 포함되는 것이 있으면 해당 PI는 EPI임
* removeRepeat
  * EPI가 반복으로 나오면 반복으로 나오는 것을 중지
* inputMinterm
  * minterm을 input 받는 함수
* inputDontCare
  * don't care을 input 받는 함수


------
