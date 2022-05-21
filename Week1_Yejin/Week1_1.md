# 1주차 발표

기간: 2022.05.07-14

질문

-모듈은 도메인 단위 

-도메인==엔티티는 아니다. 결제 도메인,,, 

도메인 설계하는 연습

공부한 내용 이야기하기?

객체지향부터 스프링까지 전반적으로 뭐를 만들지 생각하고 그걸로 공부하기?

도커,쿠버네티스,etl,,,,

숫자야구 도메인 설계하기 금요일에 도메인 공유 후 궁금한 부분 생각

### 목적

버그 걱정없이 코드를 변경할 수 있고, 변경에 유연하고 확장가능한  설계하는 방법

객체지향 프로그래밍: 데이터와 프로세스가 동일한 모듈 내부에 위치하도록 프로그래밍 하는 방식

좋은 객체지향 설계: 올바른 객체에게 올바른 책임을 할당하면서 높은 응집도와 낮은 결합도를 가진 구조를 창조하는 활동

클래스 내부와 외부 구분 & 구현 은닉 

클래스의 내부와 외부가 명확하게 구분이 되면 객체의 자율성이 증가. 

구현 은닉을 하면 클라이언트 프로그래머 → 알아야될 정보 감소

클래스 작성자 → 외부 영향 신경쓰지 않고 내부 구현 가능

캡슐화:  외부에서 알 필요가 없는 부분은 감춤으로써 대상을 단순화하는 추상화의 한 종류(변경될 수 있는 어떤 것이라도 감추는 것)

캡슐화의 목적은 객체의 자율성 확보

객체가 자신의 데이터를 처리함에 있어서 자유로워야 변경이 쉬워진다

캡슐화를 먼저 확보해야 낮은 결합도와 높은 응집도를 만들 수 있다

메시지 vs 메서드

메시지: 객체 간 상호작용을 하기 위한 유일한 방법.

메서드: 수신된 메시지를 처리하기 위한 자신만의 방법. 이는 객체가 직접 결정한다. 

다형성: 동일한 메시지를 수신했을 때 객체의 타입에 따라 다르게 응답할 수 있는 능력

장점: 타입 객체에 변경사항이 생기거나 새로운 타입을 추가해야할 때, 큰 어려움없이 변경할 수 있다. 예제 DiscountPolicy에 연결된 AmountDiscountPolicy와 PercentDiscountPolicy

상속 vs 합성

상속: 내부 구현을 그대로 사용해야하는 경우. 

부모와 자식 클래스 간의 결합이 강해져 캡슐화가 약해진다

합성: 메시지를 통해 객체가 연결되므로 느슨한 결합을 가져서 효과적으로 캡슐화 가능. 느슨한 결합으로 낮은 결합도를 가진다.