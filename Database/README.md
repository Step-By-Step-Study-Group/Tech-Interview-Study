# 💬 목차

[Transaction이란?](#transaction이란)

# Transaction이란?

트랜잭션은 은행 업무나 데이터베이스에서 더 이상 쪼개질 수 없는 최소의 작업단위를 뜻하며,
더 자세하게 데이터베이스의 트렌젝션은 데이터베이스의 상태를 변화시키기 위해서 수행하는 작업의 단위를 의미합니다.  
트랜잭션은 원자성, 일관성, 독립성, 지속성 4가지의 특징을 가지고 있습니다.(ACID)

### 원자성, Atomicity
한 트랜잭션의 연산들이 모두 성공하거나, 모두 실패하는 것을 보장하는 것을 의미합니다.  
(부분적인 성공, 실패가 없다라는 의미)
### 일관성, Consistency
데이터는 미리 정의된 규칙에서만 조작이 가능하도록 보장하는 것을 의미합니다.
### 독립성, Isolation
트랜잭션을 수행 시 다른 트랜잭션의 연산 작업이 끼어들지 못하도록 보장하는 것을 의미합니다.
### 지속성, Durability
성공적으로 수행된 트랜잭션은 영원히 반영되어야 함을 의미합니다.

### 트랜잭션의 격리 수준(Isolation Level)이란?
트랜잭션의 격리 수준이란 동시에 여러 트랜잭션이 수행될 때,
특정 트랜잭션이 다른 트랜잭션에서 변경하거나 조회하는 데이터를 볼 수 있도록 허용할지 말자를 결정하는 것입니다.  
격리 수준은 다음과 같이 4가지로 정의 할 수 있습니다.
- READ UNCOMMITTED(커밋되지 않은 읽기)
- READ COMMITTED(커밋된 읽기)
- REPEATABLE READ(반복 가능한 읽기)
- SERIALIZABLE(직렬화 가능)

순서대로 READ UNCOMMITTED의 격리 수준이 가장 낮고 SERIALIZABLE의 격리 수준이 가장 높습니다.
트랜잭션의 격리 수준이 낮을수록 더 많은 문제가 발생합니다.


[[데이터베이스] 트랜잭션의 ACID 성질](https://hanamon.kr/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98%EC%9D%98-acid-%EC%84%B1%EC%A7%88/)
[트랜잭션의 격리 수준(isolation Level)이란?](https://nesoy.github.io/articles/2019-05/Database-Transaction-isolation)