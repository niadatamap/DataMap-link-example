## 빅데이터 개방‧유통을 위한 메타데이터 구조 및 데이터 연계 규격 예시

## 개요 
- 메타데이터 조회 API 동작 예제 

## 테스트 절차
- API 요청 테스트
  - 메타데이터 목록 조회 (platformId 값을 입력시 해당 플랫폼의 메타데이터가 제외된 조회)
    ```
      $ curl -X POST \
        http://115.85.181.22:8080/api/resources/list?title=고속&platformId=1
    ```  
  - 메타데이터 상세내용 조회 (id 속성값 기준으로 상세내용 조회)
    ```
      $ curl -X GET \
        http://115.85.181.22:8080/api/resources/5388/detail
    ```
