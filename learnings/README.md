# 인프런 모든 개발자를 위한 HTTP 웹 기본 지식

### HTTP 메서드 - PUT, PATCH, DEL  
PUT은 전부 다 엎어칠 때, PATCH는 부분 변경할 때 사용한다.  

### HTTP 메서드의 속성
#### 안전(Safe)
호출해도 리소스가 변경되지 않는 것을 안전한 메서드라고 한다.   
로그 쌓여서 서버 장애 나는 것 등의 요소는 고려하지 않고,  
리소스가 변경되는지 아닌지만 생각한다.  
#### 멱등(Idempotent)
한 번 조회하든 여러번 하든 결과가 다르지 않다!  
중간에 외부 요인으로 리소스가 바뀌는 것은 고려하지 않는다.  
GET, PUT, DELETE는 멱등하지만 POST는 멱등하지 않다.  
멱등한 경우에 자동 복구 메커니즘을 사용할 수 있다!  
#### 캐시 가능(Cacheable)
모든 메서드 다 가능하지만, 보통 GET은 url만 신경쓰면 되니 GET을 많이 캐시한다.  

### 참고할만한 URL 설계 개념
#### Document
#### Collection
#### Store
#### Control URI
