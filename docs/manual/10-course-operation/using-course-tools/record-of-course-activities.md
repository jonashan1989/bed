---
sidebar_position: 8
---

# 코스 활동 기록

Learnize은 참가자 및 작성자의 코스 활동을 소위 로그 파일에 기록합니다. 데이터 보관 도구 를 사용하여 해당 로그 파일을 개인 폴더로 다운로드할 수 있습니다.

- 코스 작성자의 개인 데이터가 포함된 관리자 로그 파일
- 사용자 로그 파일 코스 참가자의 익명화된 데이터가 포함된 통계 로그 파일
- 사용자의 개인화된 활동이 포함된 사용자의 로그 파일

![log_files](/img/course-operation/log_files.png)

**개인 정보 보호**

개인 정보가 포함된 사용자 로그 파일은 개인 정보 보호를 위해 시스템 관리자만 사용할 수 있습니다.

아카이브 권한이 있는 사용자(일반적으로 코스 관리자)는 원하는 로그 파일을 ZIP 파일(예: *CourseLogFiles_2010-01-28_14-55-55.zip* )로 개인 폴더( *개인 폴더* -> *개인* -> *아카이브* )에 저장할 수 있습니다. 이 ZIP 파일에는 선택한 파일 *인 course_statistic_log.csv* , *Course_admin_log.csv* 또는 *Course_user_log.csv* 가 포함되어 있습니다 .

*Course_statistic_log.csv* 파일에서 코스 참가자는 다음과 같이 익명으로 처리됩니다. 각 코스 참가자는 무작위로 생성된 번호(예: *7FFBA8C371B1A3DACCF5F12227A75CE82D6C4CE6)를 받습니다. 이 숫자는 코스 내에서 변경되지 않습니다. 이 숫자는 과정 내내 지속됩니다. 따라서 코스 Y에서 참가자 X의 활동을 관찰할 수 있지만 참가자가 코스 Z에서 다른 번호를 받게 되므로 이러한 데이터를 코스 Z와 비교할 수 없습니다.

로그 파일 열 actionCrudType(데이터베이스 작업), actionVerb(액션) 및 actionObject(처리된 코스 객체)(정렬)에 가능한 항목:


**actionCrudType** 열 은 기본 데이터베이스 작업에서 실행된 작업을 요약합니다. 이들은 actionVerb 열에서 분류되므로 actionCrudType 열은 귀하와 관련이 없습니다. 그럼에도 불구하고 다음과 같은 작업을 수행합니다.

- C=만들기
- R=읽기/검색
- U= 업데이트/수정
- D=삭제
- E=종료

actionVerb 열은 이제 사용자("userName의)가 actionObject 열의 코스 객체로 실제로 무엇을 했는지 조사합니다. 따라서 **actionObject** 열의 항목 은 최소한 데이터베이스의 관점에서 변경되는 코스 객체를 나타냅니다.


그래서 세 번째 줄은

`u / add / participant / [group name] / [username]`

그에 따라 읽힐 것입니다(데이터베이스 작업: 업데이트/수정):

`Add user [username] to [group]`

로그 파일을 그래픽으로 분석하는 옵션은 "통계" 섹션에서 자세히 설명합니다 .