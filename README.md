# SQL-Profile
## Tibero(RDBMS)의 sql profile 기능 개선 프로젝트
+ SQL Profile 기능 설명
  + plan 변경으로 성능 저하 발생시 해당 SQL Profile(미리 저장해둔 플랜)을 찾아 원하는 plan으로 쿼리가 샐행되도록 하는 기능
  +  plan이 변경되지 않은 경우라도, SQL에 힌트를 넣어 outline을 만들고 import sql profile을 수행하면, 힌트 전 sql이 들어왔을 때, 힌트가 사용된 플랜으로 풀리도록 하는 기능
  +   [ORACLE SQL PROFILE](https://docs.oracle.com/database/121/TGSQL/tgsql_profiles.htm) 과 같은 기능이므로 자세한 설명은 링크 참조
## Tibero에 추가해야할 기능
+ Tibero에 있는 SQL Profile 기능은 일반 장애(단순 성능 저하 및 플랜 변경)에 대해서는 대응할 수 있지만 심각한 장애(DB down, 재부팅, 심각한 성능저하)에 대해서는 대응 불가
+ SQL Profile(장애를 대비한 플랜 저장)을 메모리에서만 관리하고 있어 메모리 관련 장애가 발생하면 SQL Profile을 사용할 수 없음

## Member
+ 1인 프로젝트

