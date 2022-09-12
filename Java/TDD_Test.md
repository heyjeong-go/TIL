# TDD
### TDD 란..
- TDD(Test-Driven Development) : 테스트 주도 개발
  + 매우 짧은 개발 사이클을 반복하는 소프트웨어 개발 프로세스 중 하나
  + 진행 방식 : **준비 -> 동작 -> 확인**
    * 요구 기능에 대한 테스트 코드 작성
    * 테스트 케이스를 통과하기 위한 최소한의 코드 생성
    * 리팩토링
  + 작성 방식
    * case 1 : 구현 대상 클래스의 외형에 해당하는 메소드들을 먼저 만들고 테스트 케이스를 일괄적으로 만드는 방식
    * case 2 : 테스트 케이스를 하나씩 추가해가면서 구현 클래스를 점진적으로 만드는 방식
- JUnit : 자바 프로그램의 단위 테스트를 위한 대표적인 프레임 워크
  + 현재 최신 버전은 JUnit5
- JUnit에서 지원하는 어노테이션 정리
  + @Test
    * 해당 어노테이션이 선언된 메소드는 테스트를 수행하는 메소드가 됨
    * 각각의 테스트가 서로 영향을 주지 않고 독립적으로 실행됨을 원칙으로 @Test마다 객체를 생성함
  + @Ignore
    * 테스트를 실행하지 않음
  + @Before
    * @Test 메소드가 실행되기 전에 반드시 실행됨
    * @Test 메소드에서 공통으로 사용하는 코드를 해당 메소드에 선언하여 사용하면 됨
  + @After
    * @Test 메소드가 실행된 후 실행됨
  + @BeforeClass
    * @Test메소드보다 먼저 한번만 수행되어야 할 경우에 사용됨
  + @AfterClass
    * @Test메소드보다 나중에 한번만 수행되어야 할 경우에 사용됨
  + Assert class
    * assertArraEquals(a, b) : 배열 a와 b가 일치함을 확인
    * assertEquals(a, b) : 객체 a와 b의 값이 같은지 확인
    * assertSame(a, b) : 객체 a와 b가 같은 객체임을 확인
    * assertTrue(a) : a가 참인지 확인
    * assertNotNull(a) : a객체가 null이 아님을 확인

### TDD 예제1 : 파일 생성, 쓰기, 저장
- [TDD 예제 1](https://velog.io/@heyjeong-go/Java-TDD-%EC%A7%84%ED%96%89%ED%95%B4%EB%B3%B4%EA%B8%B0)
- 2022-09-08 : 기존에 작성했던 '파일 생성 및 쓰기 구현' 프로그램을 TDD 형식으로 다시 진행해보기
  + ~~아직 제대로 된 구현 못함..~~
- 2022-09-13 : 파일 생성 부분 TDD로 구현해냄! 손 가는대로 구현...

***
### TDD 참고
> https://velog.io/@jkijki12/Java-TDD  
https://hwan1001.tistory.com/56  
https://juhi.tistory.com/38  
https://shlee0882.tistory.com/202