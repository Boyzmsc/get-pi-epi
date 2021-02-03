# PI/EPI 찾기 프로그램

**이 프로젝트는 논리회로설계 강의를 바탕으로 제작되었습니다.**

C++ 프로그래밍 언어를 이용해 제작했으며,
비트 수를 입력하고 그에 따라 입력받는 minterm과 don't care에 따른 Prime Implicants와 Essential Prime Implicants를 구하는 프로그램입니다.


## 목차

|   내용    |
| :-------: |
| 실행 방법 |
| 소스 코드 |




## 실행 방법

#### 1) 소스 파일을 컴파일 한 뒤 실행합니다.

#### 2) 비트 수를 입력합니다.

* 0 이하의 수는 받지 않습니다.

#### 3) minterm을 입력합니다.

* -1을 입력 시 입력이 종료되며, 음수나 반복된 수는 받지 않습니다.

#### 4) don't care를 입력합니다.

* -1을 입력 시 입력이 종료되며, 음수나 반복된 수는 받지 않습니다. minterm에 포함된 수도 받지 않습니다.

#### 5) 결과가 출력됩니다.

* Minterm : 입력한 minterm을 출력합니다.

* Don't care : 입력한 don't care을 출력합니다.

* Binary List : minterm과 don't care의 비트 수에 따른 이진 데이터를 출력합니다.

* Prime Implicants : PI를 출력합니다.

* One repeat Minterm : minterm과 don't care중에서 한번만 나오는 요소들을 출력합니다.

* Final One repeat Minterm : don't care을 제외한 한번만 나오는 minterm들을 출력합니다.

* Essential Prime Implicants : EPI를 출력합니다.

#### 6) 출력 화면

![screenshot](https://user-images.githubusercontent.com/28584213/99257128-de32be80-2859-11eb-8aa8-2d6cf48b974d.png)
