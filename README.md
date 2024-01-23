# SQL-Profile
## Tibero의 sql profile 기능 개선 프로젝트
## SQL Profile 기능 설명
### plan 변경으로 성능 저하 발생시 해당 SQL Profile(미리 저장해둔 플랜)을 찾아 원하는 plan으로 쿼리가 샐행되도록 하는 기능
### plan이 변경되지 않은 경우라도, SQL에 힌트를 넣어 outline을 만들고 import sql profile을 수행하면, 힌트 전 sql이 들어왔을 때, 힌트가 사용된 플랜으로 풀리도록 하는 기능
### [ORACLE SQL PROFILE](https://docs.oracle.com/database/121/TGSQL/tgsql_profiles.htm)과 같은 기능
