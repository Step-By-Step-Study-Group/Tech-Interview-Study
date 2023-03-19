# 💬 목차

- [스프링과 스프링 부트의 차이점](#스프링과-스프링-부트의-차이점)
- [Spring MVC와 Spring Webflux](#Spring-MVC와-Spring-Webflux)

# 스프링과 스프링 부트의 차이점

### Spring
> 엔터프라이즈용 JAVA 애플리케이션 개발을 편하게 할 수 있게 해주는 오픈소스 경량급 애플리케이션 프레임워크

### 특징
#### POJO 프로그래밍을 지향
스프링의 가장 큰 특징으로 볼 수 있습니다. 여기서 POJO란, Plain Old Java Object, 즉 순수 Java만을 통해서 생성한 객체를 의미합니다.
그렇다면 순수 Java만을 통해 객체를 만든다는게 무슨 의미일까요?

순수 Java만을 사용한다는 것은 **Java 및 Java의 스펙에 정의된 기술만 사용한다라는 의미**입니다. 즉, 어떤 객체가 외부의 라이브러리나 외부의 모듈을 가져와서 사용하고 있다면, 그 객체는 POJO라고 할 수 없습니다.

#### POJO는 왜 중요한가?
POJO는 순수 Java만을 사용하여 만득 객체이므로 특정 기술이나 환경에 종속되지 않습니다. 따라서, 외부 기술이나 규약의 변화에 얽매이지 않아, 보다 유연하게 변화와 확정에 대처할 수 있다는 장점이 있습니다. 이처럼 비즈니스 로직을 구현하는 데에 POJO를 적극적으로 활용하는 프로그래밍 패러다임을 **POJO 프로그래밍**이라고 합니다.

### Spring Boot
> 스프링은 기존 기술의 복잡성을 크게 줄인 프레임워크이지만, 그럼에도 불구하고 스프링을 사용하기 위해서는 여러가지 설정이 필요합니다. 스프링 부트는 이러한 기존의 스프링이 가지고 있는 복잡하고 반복되는 설정을 대신 해주는 별도의 프레임워크입니다.

기존 스프링을 통해 개발을 하고 배포를 하려면 별도의 외장 웹 서버를 설치하고, 프로젝트 .war 파일로 빌드하여 배포를 진행하였습니다. 이러한 방식은 처리 속도가 느리며 번거롭다는 단점을 가지고 있습니다.
반면, 스프링 부트는 자체적인 웹 서버를 내장하고 있어(Tomcat), 빠르고 간편하게 배포를 진행할 수 있습니다. 또한, 독립적으로 실행 가능한 .jar 파일로 프로젝트를 빌드할 수 있어, 클라우드 서비스 및 도커와 같은 가상화 환경에 빠르게 배포할 수 있습니다.

### Reference
- [스프링과 스프링부트(Spring Boot)ㅣ정의, 특징, 사용 이유, 생성 방법](https://www.codestates.com/blog/content/%EC%8A%A4%ED%94%84%EB%A7%81-%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8)
- [[Spring] Spring과 Spring Boot의 차이점, Hibernate, Bean Scope, Bean 생명주기](https://yamyam-spaghetti.tistory.com/56)

# 스프링 빈이란 무엇이며 빈 등록은 어떻게 할 수 있는가.
### 빈(Bean)이란 무엇인가

빈이란 **스프링 IoC 컨테이너가 관리하는 자바 객체를 의미**합니다.
여기서 말하는 자바 객체는 POJO 자바 객체를 의미합니다.

### IoC 컨테이너에 빈 등록하기
#### 1. 어노테이션(Annotation)을 사용하는 방법
`@Component` 어노테이션을 사용하는 방법이 있습니다.
`@Component` 어노테이션이 붙어 있는 경우 컴포넌트 스캔을 통해 빈으로 등록해줍니다.
스테레오 타입(Stereotype)인 `@Controller`,`@Service`,`@Repository`와 같은 어노테이션은 내부에 `@Component` 어노테이션을 가지고 있는 합성 어노테이션으로 컴포넌트 스캔시에 스캔되는 어노테이션입니다.

#### 2. 빈 설정 파일에 직접 등록하는 방법
해당 방법은 `@Configuration`과 `@Bean` 어노테이션을 사용합니다.
`@Configuration` 어노테이션의 경우 간단하게 말하면 "해당 파일에 빈을 등록할 것이니 조회해줘"라는 표시입니다.
`@Configuration` 어노테이션이 붙은 파일 내에서 `@Bean` 어노테이션을 사용해서 빈을 직접 등록하게 되는데, `@Bean`을 사용해 수동으로 등록할 때에는 해당 메서드 이름이 빈 이름으로 결정됩니다.

> 스프링의 경우 컴포넌트 스캔을 통해 자동으로 빈 등록을 하는 방식을 권장합니다.
Spring에서는 Main App 클래스에서 `@ComponentScan` 어노테이션을 사용해서 등록해야하며,
Spring Boot 환경에서는 디폴트로 존재하는 `@SpringBootApplication` 어노테이션 내부에 `@ComponentScan` 어노테이션이 포함되어 있습니다.

### Reference
[[Spring] 스프링 빈(Bean)이란?](https://mozzi-devlog.tistory.com/19)
[[Spring] Spring Bean 총 정리](https://steady-coding.tistory.com/594)

# Spring-MVC와-Spring-Webflux
**Spring MVC**는 우리가 Spring Boot를 쓰면 사용하게 되는 가장 보편적인 방식으로 볼 수 있다.
Spring MVC는 요청이 들어오면 그 때마다 Thread를 생성한다. 결국 다수의 요청이 오면 그만큼의 Thread를 생성해야 하고 리소스가 굉장히 많이 들아가게 된다. 그래서 Spring MVC는 애플리케이션이 실행되면 Thread pool을 생성하고 요청이 들어오면 Thread pool에 Thread들이 요청을 하나씩 가져가게 된다.
이 방식의 단점은 요청의 수가 pool size를 초과하면 요청이 계속 쌓이게 되고 Thread Pool Hell 현상이 발생할 수 있는 점이다..

**Spring WebFlux**는 Event driven 방식이고 비동기 논블로킹 방식이라고 한다. Node.js처럼 이벤트 루프가 돌아서 요청이 발생하면 그것에 맞는 핸들러가 처리를 위임하고 처리가 완료되면 callback메소드를 통해 응답을 반환한다. 따라서 적응 thread로도 많은 사용자의 요청을 받아낼 수 있다.  
단순히 생각해보면 Webflux방식을 사용하는 것이 더 좋아보일 수 있지만 WebFlux방식의 성능을 끌어내려면 요청을 처리하는 모든 파이프라인이 논블로킹하게 동작해야만 한다. 특정 구간에 블로킹 방식이 있으면 거기서부터 Thread Pool Hell같은 문제들이 역시 발생할 수 있다.

**Thread pool hell** : 설정해놓은 thread pool size를 넘게 되면 작업이 처리될 때까지 Queue에서 계속해서 기다려야 한다. 그래서 전체의 대기시간이 늘어나는데 이런 현상을 **Thread pool hell** 이라고 한다.