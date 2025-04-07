# Redis
## 로컬 레디스 전 후 측정
### 레디스(캐싱) 전 측정
![image](https://github.com/user-attachments/assets/b90745e9-c3d4-4710-90ef-1fc5264b4136)

### 레디스(캐싱) 적용 후
![image](https://github.com/user-attachments/assets/7792ec03-909c-4346-9b4a-d727b2eb1ecf)


## 부하 테스트
- 백엔드 서버를 구현하고 나서 배포를 하게 된다. 실제 서비스에 사용자 요청을 견딜 수 있는지 부하 테스트를 해야한다.
- 부하 테스트에서 서비스가 1초당 처리할 수 있는 작업량을 보고 Throughput이라고 부른다. 단위는 TPS(Transaction Per Seconds, 1초당 처리한 트랜잭션의 수)를 많이 활용한다. 만약 내가 만든 서비스가 1초에 최대 100개의 API 요청을 처리할 수 있다면, 이 서비스의 Throughput은 100 TPS라고 얘기 한다.

### 레디스(캐싱) 전 측정
![image](https://github.com/user-attachments/assets/9ac25af2-7ddd-4549-aee3-59add8f29820)
- 레디스 전 Trougput은 3.0TPS(1초당 3개 요청을 처리 할 수 있다)


### 레디스(캐싱) 후 측정
![image](https://github.com/user-attachments/assets/c00b364c-dc26-48d4-9064-a68a11961ec0)
- 레디스 후 Trougput은 25.3TPS(1초당 25.3개 요청을 처리 할 수 있다)
