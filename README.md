# Practice

>  start : 2018-10-09
>
>  참고 : 『자바스크립트 프로젝트 북』 , 한빛미디어 , 권대용 , 2017



## p1. 달력

> Date() 객체를 이용한 달력 만들기
>
> 작업 파일 : calendar.html



## p2. 지도

> 오픈 API인 구글 맵을 활용하여 지도 만들기
>
> 작업 파일 : map.html 참고 사이트 :  [GOOGLE Maps Platform](https://developers.google.com/maps/documentation/javascript/tutorial)



## p3. 날씨 위젯

> openweather API 를 이용하여 위젯 형태의 어플리케이션 구현
>
> 작업 파일 : weather.html
>
> 참고 : [openweather](https://openweathermap.org/current)



## p4. 퀴즈 게임

> 객체 지향 프로그래밍을 활용한 사지선다형 퀴즈 게임 구현
>
> 유지보수를 위해 문제와 퀴즈 진행 정보 등을 자료화시켜 처리


## p5. 회원가입 폼

> if문을 이용한 유효성 검사 구현
>


## 새로 알게 된 개념

##### 오픈 API 

Application Programing Interface / 이용자가 직접 응용 프로그램을 개발할 수 있도록 공개된 개발용 프로그래밍 라이브러리



##### AJAX

AJAX 는 비동기 통신 처리를 의미하며, 웹 브라우저 측에서 자바스크립트를 통해 필요한 부분만 서버에 요청하고 나머지 부분은 비동기적으로 처리하는 방식이다. 

기존 동기화 방식이 A를 시작하고 결과를 확인한 후에 B를 진행하는 형태였다면, 비동기 처리 방식은 A의 결과가 나오지 않아도 바로 A에 대한 결과 처리 부분은 별도의 테이블에 맡겨둔 뒤 다음 B를 실행하는 방식이다. 

그 결과 비동기 프로그래밍 방식은  동기화 프로그래밍 방식에 비해 더 빠르게 작업을 처리할 수 있다.

** AJAX는 로컬 서버 환경 설정 후 테스트가 가능하다.



##### XML

HTML과 같이 태그 구조의 형식으로 데이터를 표현한다.  데이터 이외의 열고 닫는 태그가 반드시 필요하므로 구조가 복잡해지고 용량이 커지게 되는 단점이 있다.



##### JSON

자바스크립트 객체 데이터 형식 (JavaScript Object Notation) 으로 XML 데이터 형식에 비해 구조 정의의 용이성과 가독성이 뛰어나 AJAX의 표준으로 사용.

```
{
    "book": [
    	{
            "title": "채식주의자";
            "autor": "한강";
            "price": "12000";
    	},
    	{
            "title": "종의 기원";
            "autor": "정유정";
            "price": "13000";
    	}
    ]
}

```



##### 객체

객체 : 작업의 대상

객체 지향 : 객체를 새롭게 정의하는 것

객체 기반 : 기존에 만들어진 객체를 사용하는 것

-> JavaScript는 객체 기반 언어이면서 객체 지향 언어이기도 하다. (객체 지향은 변수나 함수를 더 구조적으로 표현해야할 때 사용되며 차후 유지 보수가 쉽다.) 또한 객체 지향 프로그래밍의 특징은 기존 변수와 함수가 자료 처리 중심에서 벗어나 객체라는 단위로 설계됨으로써 서로 결합하고 상호 작용한다는 점이다.

ex) 캐릭터라는 객체(Object) 에는 직업:기사, 나이:25와 같은 속성(Property) 가 있으며, 움직이거나 달리는 메서드(Method)를 정의할 수 있다.

```
var charactor = {
	name: '감자',
	job: '탱커',
	move: function(){
		document.write('캐릭터 이동<br>');
	},
	stop: function(){
		document.write('캐릭터 정지<br>');
	}
} // 이 때 name, job이 charactor의 속성, move, stop이 메서드
```



그러나 속성은 생성되는 인스턴스마다 각기 다른 값을 적용시켜야 하는 반면, 메서드는 모든 인스턴스마다 공통으로 사용으로 하기 때문에 속성은 '생성자 함수'에, 메서드는 '프로토타입 속성'으로 정의하는 것이 좋다. 



