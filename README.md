# ORM : jpa
## ORM(Object-relational mapping) 이란 객체 관계 매핑이다.
객체는 객체대로 설계하고, 관계형 데이터베이스는 관계형 데이터베이스대로 설계한다.
ORM 프레임워크가 중간에서 매핑해준다.
대중적인 언어에는 대부분 ORM 기술이 존재한다.
ORM은 객체와 RDB 두 기둥 위에 있는 기술 이다.
JPA(Java Persistence API)란 ORM 기술 표준으로, 실제로 동작하는 것이 아니라 인터페이스의 모음이다.

EJB : 과거의 자바 표준 (Entity Bean) ORM
Hibernate : ORM 프레임워크, Open Source SW EJB2 스타일의 Entity Beans 이용을 대체할 목적으로 개발하였다.
JPA 표준 명세를 구현한 3가지 구현체로는 Hibernate, EclipseLink, DataNucleus가 있다. 이 중에서 JPA 인터페이스를 구현한 대표적인 오픈소스가 Hibernate라고 할 수 있다.

## 왜 JPA를 사용해야 하는가?
JPA를 자바 컬렉션에 객체를 저장하듯 JPA에게 저장할 객체를 전달.
INSERT SQL을 작성하고 JDBC API 사용하는 지루하고 반복적인 일을 JPA가 대신 처리해준다.
CREATE TABLE같은 DDL문 자동 생성
데이터베이스 설계 중심의 패러다임을 객체 설계 중심으로 역전

Data JPA -참고합니다 ==>  https://docs.spring.io/spring-data/jpa/docs/1.10.1.RELEASE/reference/html/#jpa.sample-app.finders.strategies

## JPQL이란?
엔티티 객체를 조회하는 객체지향 쿼리이다.
문법은 SQL과 비슷하고 ANSI 표준 SQL이 제공하는 기능을 유사하게 지원한다.
SQL은 데이터베이스 테이블을 대상으로 JPQL은 엔티티 객체를 대상으로 쿼리 한다.
JPQL은 SQL을 추상화해서 특정 데이터베이스에 의존하지 않는다.
JPQL은 최종적으로 SQL로 변환된다.

JPQL 사용 : 참고합니다 ==> https://jang8584.tistory.com/282
