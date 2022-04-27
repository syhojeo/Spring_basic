# Bean 의 태그 및 객체 생성

# Bean 객체 생성

## Bean 태그

사용할 Bean을 정의하는 태그

## bean 태그의 기본 속성

### class

객체를 생성하기 위해 사용할 클래스

### id

객체를 가져오기 위해 사용하는 이름

id가 다를경우 다른 객체로 생각하여

싱글톤 특성을 가지는 ApplicationContext의 경우에 같은 클래스를 지정한다고 해도 id가 다를 경우 객체를 계속해서 생성한다

### lazy-init

싱글톤인 경우 xml을 로딩할 때 객체 생성 여부를 설정

true 일 경우 xml 로딩 시 객체를 생성하지 않고, 객체를 가져올때 생성한다

### scope

객체의 범위를 설정한다

singleton - 객체를 하나만 생성해서 사용한다

prototype - 객체를 가져올 때 마다 객체를 생성한다