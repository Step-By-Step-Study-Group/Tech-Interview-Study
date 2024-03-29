# 💬 목차

[동기와 비동기의 차이](#동기와-비동기의-차이)  
[동시성과 병렬성의 차이](#동시성과-병렬성의-차이)

## 동기와 비동기의 차이

### 동기

특정 작업을 수행할 때 해당 작업이 완료될 때까지 대기하며 다른 작업을 수행하지 않음

- 설계가 간단하고 직관적
- 현재 작업의 결과를 기다리는 동안 다른 작업을 처리할 필요가 없어 자원 낭비하지 않음
- 결과가 주어질 때 까지 아무것도 못하고 대기해야함( 멀티태스킹 x )

### 비동기

여러 작업을 동시에 처리하며 각 작업이 완료될 때까지 기다리지 않음

- 설계가 복잡하고 구현이 어려움
- 작업하는 동안 다른 작업을 할 수 있으므로 자원을 효율적으로 사용 가능
- 처리작업시 동시에 처리되는 작업이 많아질경우 부하가 생길수있어 관리가 필요함  
<br>
<br>  
  
# 동시성과 병렬성의 차이  
  
|동시성(Concurrency)|병렬성(Parallelism)|  
|:---:|:---:|
|여러 작업이 동시에 실행되고 있는 것처럼 구현되는 것|여러 작업이 실제로 동시에 실행되고 있는 것|  
|싱글 코어 환경에서 단일 프로세스 내에 멀티 스레드를 동작하여 구현|멀티 코어 환경에서 멀티 프로세스(단일 스레드) 혹은 멀티 스레드를 활용하여 처리|  
|빠른 시간에 하나씩 많은 것을 처리|한번에 많은 것을 처리|  
|논리적인 부분|물리적인 부분|  
|예시)커피 추출구가 하나인 커피머신이 아메리카노, 라떼, 마끼야또를 재료를 바꿔가면서 동시에 만들어지도록 구현.|예시)커피 추출구가 여러개인 커피머신이 동시에 각각의 재료를 통해 아메리카노, 라떼, 마끼야또를 만듬.|    
<br>  

**동시성(Concurrency)** 은 여러 작업이 겹치는 기간에 실행될 수 있음을 의미한다. 동시에 실행하는 것이 아니라 CPU가 작업마다 시간을 분할해 적절하게 context switching을 해서 동시에 실행되는 것처럼 보이게 한다. 이렇기 때문에 동시성은 구현하는 것도 디버그하는 것도 어렵다.  
  
동시성의 핵심 목표는 유휴 시간을 최소화하는 것이다. 유휴 시간은 컴퓨터가 작동 가능한데도 작업을 하지 않는 시간으로 아무것도 안하고 놀고 있는 시간이라고 생각하면 된다. 현재 프로세스 또는 스레드가 I/O 작업, DB 트랜잭션 등등 외부 프로그램 실행을 기다리는 동안에 다른 프로세스 또는 스레드가 CPU 할당을 받는다.  
<img width=750 src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fuuu7O%2FbtrLMAgBO6G%2FiWueIGWBR8ojEwfqk86jek%2Fimg.png">  
이 여러개의 task들은 하나 이상의 코어에서 실행된다. 같은 시간에 같은 자원에 접근하는 상황이 생길 수 있는데 해당 자원에 write 권한으로 접근하는 경우 **데이터의 무결성 유지**를 염두해야 한다.  
  
<br>  

**병렬성(Parallelism)** 은 동일한 시간에 독립적인 작업을 실행할 수 있음을 의미한다. 동시성과는 달리 여러 작업을 다른 코어, 다른 프로세스, 별도의 컴퓨터 등에서 동시에 실행할 수 있다. 그래서 병렬 처리가 성능 향상에 필수적이라고도 한다.  
  
한가지 예로 분산 컴퓨팅 시스템이 있다. 분산 컴퓨팅 시스템은 단일 시스템으로 실행하는 여러 컴퓨터 시스템들로 구성되어 있다. 각 컴퓨터에 존재하는 시스템들은 네트워크로 연결될 수 있다.  
<img width=750 src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FMQ6QI%2FbtrLLW5YO0c%2F51DDn21VhVYb7H1mMYsw00%2Fimg.png">
