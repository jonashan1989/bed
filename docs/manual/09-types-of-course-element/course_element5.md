# 기타

- 1 기타
    - 1.1 코스 요소: LTI 페이지
    - 1.2 코스 요소: 주제 할당
    - 1.3 코스 요소: 링크 목록
    - 1.4 코스 요소 "날짜 지정"

## 과정 요소: LTI 페이지

![basiclti](/img/course_elements/basiclti.png)

코스 요소 "LTI 페이지"를 통해 Learnize 창에 콘텐츠가 표시되기 전에 코스에 외부 학습 애플리케이션을 통합할 수 있습니다. LTI는 "학습 도구 상호 운용성"을 의미하며 채팅, 미디어 Wiki, 테스트 편집기 또는 가상 랩과 같은 외부 학습 응용 프로그램을 포함하기 위한 IMS 표준입니다. LTI에 대한 자세한 정보는 LTI 프로젝트 페이지에서 확인할 수 있습니다.

키 및 암호와 함께 "페이지 콘텐츠" 탭에서 참조할 URL을 지정합니다. 코스 탐색에서 이 LTI 페이지를 선택할 때 사용자는 먼저 개인 정보 보호를 위해 데이터 전송을 수락해야 사용자 데이터, 코스 정보 또는 키가 백그라운드에서 암호로 제어되는 임베디드 애플리케이션으로 전송됩니다. 학습 응용 프로그램은 액세스 권한을 확인하고 유효한 키로 액세스 권한을 부여합니다. 데이터 전송을 위한 새로운 쿼리는 전송된 데이터와 관련하여 장치의 구성이 변경된 경우에만 나중에 다시 발생합니다.

사용자가 탐색에서 LTI 페이지를 선택하면 통합 학습 응용 프로그램이 Learnize 코스에 나타납니다.

LTI 구성 페이지

다음 매개변수를 구성할 수 있습니다.

**URL: "** http://....." 형식으로 외부 학습 애플리케이션의 주소를 표시하십시오 . 

**키:** 외부 학습 애플리케이션 공급자가 제공한 키를 표시하십시오(위의 예에서는 "lti_quiz"가 됨).

**암호:** 외부 학습 응용 프로그램의 공급업체에서 제공한 키에 해당하는 암호를 지정하십시오(위의 예에서는 "weeHoo1w").

**시작 페이지 건너뛰기:** 이 옵션이 활성화되면 "LTI 학습 콘텐츠 표시" 중간 페이지 없이 연결된 응용 프로그램이 직접 표시됩니다. 관리자는 이 옵션을 비활성화할 수 있습니다.

---

**이름/이름 전송:** 이 확인란을 선택하면 사용자의 성과 이름이 외부 학습 애플리케이션으로 전송됩니다. 그렇지 않으면 사용자가 이 응용 프로그램을 익명으로 사용할 수 있습니다.

**이메일 주소 전송:** 이 확인란을 선택하면 사용자의 이메일 주소가 외부 학습 애플리케이션으로 전송됩니다.

**추가 속성** : 이 입력 상자 안에 학습 애플리케이션으로 전송되어야 하는 추가 매개변수를 추가할 수 있습니다. 예를 들어 이 학습 애플리케이션에 학습 플랫폼 Learnize에서 쿼리를 전송하도록 지시할 수 있습니다. (외부 학습 애플리케이션은 이러한 전송된 정보를 처리할 수 있어야 하므로 제공자와의 동의가 필요합니다.) 텍스트 속성(각 사용자에 대해 동일한 값)과 추가 동적 사용자 속성(각 사용자마다 다름) 중에서 선택할 수 있습니다. 사용자). 원하는 만큼 속성을 추가할 수 있지만 LTI 리소스는 표준에 지정되어 있지 않기 때문에 어떤 속성이 전송되는지 알아야 합니다.

---

**Learnize 역할** : 여기에서 LTI 리소스를 시작할 때 사용자가 갖게 될 역할을 구성할 수 있습니다. 세 가지 Learnize 역할 Author, Coach 및 Participant가 지원됩니다. 각 역할에 대해 매핑은 LTI 리소스의 해당 역할에 정의될 수 있습니다. 다음 LTI 역할을 사용할 수 있습니다. 학습자, 강사, 관리자, 조교, 콘텐츠 개발자 및 멘토 .

---

**점수 전송** : LTI 리소스가 LTI 1.1 표준을 사용하여 Learnize에 전송할 수 있는 점수 값을 생성하는 경우 이 확인란을 선택합니다. 이것은 선택 사항입니다. 제출된 점수는 LTI 과정 요소의 사용자 시작 화면과 이 과정의 효율성 설명에 나타납니다. LTI 표준에 따르면 0과 1 사이의 값만 허용됩니다.

"점수 이전" 옵션이 활성화된 경우 LTI 페이지를 평가 가능한 코스 요소로 코스에 추가할 수 있으며, 이는 평가 도구에 나타납니다. 그 외에도 LTI 과정 요소의 홈페이지에도 점수가 표시됩니다.

**스케일링 팩터** : 스케일링 팩터를 사용하면 LTI 사양에 따라 0과 1 사이의 값을 가져야 하는 LTI 결과를 Learnize 코스에 대해 보다 실용적인 값으로 스케일링할 수 있습니다. 예를 들어, LTI 시험이 Learnize에서 최대 10점을 가지도록 하려면 배율 인수를 "10"으로 지정해야 합니다. 전송된 점수를 수정하지 않으려면 계수 "1"을 사용하십시오.

**합격에 필요한 점수** : 여기에서 LTI 과정 요소가 합격으로 간주되는 시기를 정의하기 위해 선택적 컷 값을 구성할 수 있습니다. 컷 값은 LTI에서 전송한 원시 값이 아니라 스케일링 후의 점수 값과 관련이 있습니다. 위의 예에서 "5"의 절단 값은 "50%"와 같습니다.

---

**표시** : 코스 레이아웃에 LTI 리소스를 포함하려면 "코스에 포함(iFrame)" 옵션을 선택합니다. "모듈만 표시, LMS(iFrame) 숨기기" 옵션은 LTI 모듈이 활성화되어 있는 동안 Learnize을 완전히 숨깁니다. "새 창에서 열기" 옵션을 사용하면 LTI 리소스가 별도의 창에서 열립니다. 리소스에 많은 공간이 필요하거나 다른 코스 요소와 병행하여 사용해야 하는 경우에 유용할 수 있습니다.

**디스플레이 높이** : "자동" 또는 자동 기능이 제대로 작동하지 않을 경우 명시적 크기를 선택합니다.

**디스플레이 너비** : "자동" 또는 자동 기능이 제대로 작동하지 않을 경우 명시적 크기를 선택합니다.

---

**실행 시 전송된 모든 정보 표시(디버그)** : 이 확인란을 선택하면 다른 사용자가 전송된 정보를 볼 수 있습니다. 이 정보에는 사용자 식별, 코스 제목, 코스 요소 등과 같은 매개변수가 포함됩니다. 전송된 데이터 디스플레이 상단의 코스 보기에서 "Launch Endpoint with BasicLTI Data"를 클릭하면 학습 애플리케이션의 홈페이지로 이동합니다. .

## 코스 요소: 주제 할당

![projectbroker](/img/course_elements/projectbroker.png)

코스 요소 "주제 할당"은 감독을 받기 전에 코스의 학기 논문에 대한 주제를 발표하려는 경우에 유용합니다. 코스 작성자는 주제 할당의 세부 구성을 결정합니다. 이것은 예를 들어 누가 주제를 발표하고 감독할 권한이 있는지, 주제가 어떻게 설명되어야 하는지 또는 한 코스 참가자가 선택할 수 있는 주제 수로 구성됩니다. 이 코스 요소를 특별하게 만드는 것은 코스 작성자가 아니라 주제 작성자가 이러한 주제를 발표하고 감독한다는 사실입니다.

### 편집기 보기

### **주제 할당을 구성하는 방법**

"구성" 탭에서 한 참가자가 선택할 수 있는 주제 수를 먼저 결정합니다. 이 선택이 확실하거나 주제 작성자가 먼저 수락해야 합니다. 또한 추가 필드를 추가하여 주제를 더 자세히 설명할 수 있습니다. 이 설명은 발표된 모든 주제가 포함된 테이블에 표시됩니다. 여기에서 등록 및 제출이 특정 기간 내에만 가능한지 여부도 결정할 수 있습니다. "하위 요소" 탭에서 주제 할당에 드롭 상자와 반환 상자가 있어야 하는지 여부를 선택할 수 있습니다. 그러면 코스 참가자는 파일을 해당 보관함에 업로드하고 주제 작성자는 반환 상자를 통해 해당 파일을 반환합니다.

구성

**참가자당 주제 수를 제한하시겠습니까?:** 이 옵션을 선택하면 참가자가 코스 요소 주제 할당에서 선택할 수 있는 주제 수를 나타내는 필드가 나타납니다.

**주제 작성자는 참가자를 수락해야 합니다.** 이 옵션을 선택하면 참가자는 일시적으로 주제에 대해서만 등록할 수 있습니다. 주제 작성자는 최종적으로 후보자를 수락하기 전에 후보자를 선택해야 합니다.이 옵션을 선택 취소하면 이 주제에 대해 이미 등록된 모든 참가자가 자동으로 수락됩니다. 그러나 주제 작성자는 먼저 최대 참가자 수를 정의할 수 있습니다.

**하나의 주제만 허용됨(승인된 참가자는 다른 주제에서 자동으로 로그아웃됨):** 이 옵션을 선택하면 참가자로 승인된 모든 사용자가 이전에 선택한 다른 모든 주제에서 자동으로 로그아웃됩니다. 이는 참가자가 하나의 주제에 대해서만 등록할 수 있음을 의미합니다.

**추가 필드 추가:**

"필드 추가"를 통해 필요에 따라 필드를 생성할 수 있습니다. 자세한 내용을 보려면 최대 5개의 추가 필드를 만들 수 있습니다.

"이름" 필드에서 선호하는 필드 이름을 지정할 수 있습니다.

주제 작성자에게 풀다운 메뉴에 표시되는 사전 정의된 값 선택을 제공할 수 있습니다. "값" 필드에 해당 옵션을 세미콜론이나 줄 바꿈으로 구분하여 표시하십시오. 자유 텍스트 필드를 사용할 때 "값" 필드를 비워 둘 수 있습니다. 주제 작성자는 자신이 선택한 값을 채울 수 있습니다.

"표에 나타남"을 선택하면 요청한 대로 이 필드가 개요에 표시됩니다. 그 외에도 이 정보는 자세한 주제 설명에 표시됩니다.

"필드 삭제"를 통해 추가 필드를 삭제할 수 있습니다.

![Themenvergabe_Zusatz_EN](/img/course_elements/Themenvergabe_Zusatz_EN.png)

**날짜 관리:**

주제 작성자가 처리할 날짜를 선택할 수 있습니다.

**등록 날짜:** 주제 작성자는 주제에 대한 등록 마감일을 결정할 수 있습니다. 이 마감일이 지나면 참가자는 더 이상 해당 주제를 선택하거나 선택 취소할 수 없습니다. 그러나 주제 작성자는 여전히 참가자를 로그인 또는 로그아웃할 수 있습니다.

**마감: 마감** 후 보관함은 폐쇄됩니다. 그러면 참가자는 더 이상 해당 보관용 계정에 문서를 업로드할 수 없습니다.

"표에 나타남"을 선택하면 이벤트가 개요에 표시됩니다.

주제 할당에 대한 추가 설정

### **주제 작성자를 지정하는 방법**

"담당자" 탭에서 주제를 발표하고 감독할 수 있는 Learnize 사용자를 추가합니다. 이러한 사람들이 반드시 저작자 권리를 보유할 필요는 없습니다.

이미 주제를 발표한 주제 작성자를 제거하면 그는 계속해서 주제를 감독할 수 있습니다. 그러나 이 사람은 더 이상 새 주제를 발표할 수 없습니다.

### **주제 작성자의 역할**

코스 작성자가 주제 작성자로 활동하도록 승인하면 주제를 발표하고 감독할 수 있습니다. 코스 보기를 열고 주제 할당으로 이동하기만 하면 됩니다. . 주제 책임자로서 해당 주제를 편집하거나 참가자를 관리하거나 해당 주제에 대한 책임자를 더 추가할 수 있습니다. "감독 대상 그룹" 상자에 귀하가 담당하는 그룹이 표시됩니다.

### **요소 선택**

여기에서 강의 요소 주제 할당에서 Drop box 및 Return box 요소를 활성화해야 하는지 결정할 수 있습니다. 보관함에서 참가자는 파일을 업로드할 수 있습니다. 주제 작성자는 반환 상자에 파일을 저장할 수 있습니다. 수정 사항이 없으면 모든 요소가 활성화됩니다. 드롭 상자의 선택을 취소하면 해당 탭이 흐리게 표시되고 더 이상 액세스할 수 없습니다.

### **제출 확인**

파일을 성공적으로 전달한 후 새 창에서 사용자에게 표시할 텍스트를 선택적으로 입력할 수 있습니다. 텍스트를 입력하지 않으면 다음 메시지(또는 이와 유사한)가 나타납니다. 이것은 John Miller(jmiller)가 21-09-04 00:14:42에 "test.html" 파일을 보냈음을 확인하기 위한 것입니다.

*이메일로 텍스트 추가 보내기* 옵션을 선택하면 사용자는 파일을 성공적으로 제출한 후 위에서 언급한 확인 이메일을 받게 됩니다.

### 코스 보기

### **새 주제를 만드는 방법**

코스 소유자 또는 주제 관리자는 새 주제를 설정할 수 있습니다. 학습자에게 코스 내에서 주제(제안)를 설정할 수 있는 권한을 부여하면 코스 구성 방법을 결정하는 데 도움이 되거나 잠재적인 숙제나 프레젠테이션에 대한 제안을 제출할 수 있습니다.

"새 주제 만들기"를 클릭하고 주제 제목과 설명을 입력합니다. 주제 할당 구성에 따라 추가 세부 정보로 주제를 설명하고 등록 및 제출 마감일을 설정하고 얼마나 많은 코스 참가자가 주제를 선택할 수 있는지 결정하고 필요한 경우 첨부 파일로 추가 파일을 업로드할 수 있습니다. 또한 참가자가 주제를 선택 취소할 수 있는지 여부와 주제를 선택하거나 선택 취소할 때 해당 주제를 담당하는 사람에게 전자 메일로 통지해야 하는지 여부를 결정합니다.

나중에 구성을 변경하려면 주제 제목을 클릭하십시오. 이제 주제를 편집하고 주제 상태를 "무료"에서 "사용함"으로 또는 그 반대로 변경하거나 주제를 삭제할 수 있습니다.

주제를 자세히 만들고 편집합니다.

**주제:** 주제를 통해 담당자가 편집할 수 있는 주제 제목을 찾을 수 있습니다.

**담당자:** 여기에 주제 작성자 목록이 있습니다. 이 저자의 이름을 클릭하면 방문 카드로 이동하여 연락할 수 있습니다.

주제를 만들 때 자동으로 이 주제를 담당하는 사람이 됩니다. 그러나 참가자 관리 탭에서 해당 역할을 담당하는 다른 사람을 지정하거나 주제를 담당하는 사람에게 다른 사용자를 지정할 수 있습니다.

**설명: 설명** 필드에는 이 주제에 대한 자세한 정보가 포함되어 있습니다.

**주제 상태:** 이 필드는 주제 상태를 자동으로 표시합니다.

주제 관리자 또는 코스 작성자이고 주제에 대해 아직 등록한 참가자가 없는 경우 주제 상태는 "확인할 참가자 없음"으로 설정됩니다. 참가자가 이미 등록된 경우 상태는 "참가자 확인"으로 설정됩니다. 가능한 후보자 중에서 참가자를 이미 선택한 경우 "참가자 수락" 상태가 표시됩니다.

**공석 수(채움/전체):** 주제 작성자는 공석 수를 제한할 수 있습니다.

**주제 구독 취소 허용:** 활성화된 경우 참가자는 주제 구독을 취소할 수도 있습니다.

**추가 필드:** 코스 작성자가 정의할 수 있는 소위 "추가 필드"가 있습니다. 코스 작성자는 주제 작성자가 풀다운 목록에서 소위 "주제 할당: 추가 필드 추가" 값 내에서 선택해야 하는지 또는 자신의 값을 표시해야 하는지를 결정합니다. 여기에서 자유 텍스트를 표시하거나 목록에서 값을 선택할 수 있습니다.

**등록 기한:** 주제 작성자가 등록 기한을 정의하면 특정 기간 내에만 주제를 선택하거나 선택 취소할 수 있습니다. 마감일 전후에 "선택" 및 "선택 취소" 링크가 비활성화됩니다. 사용자는 귀하의 주제에 로그인하거나 로그아웃할 수 없습니다. 그럼에도 불구하고 해당 주제를 담당하는 사람은 사용자를 수동으로 로그인하거나 로그아웃할 수 있습니다.

**마감일:** 주제 작성자가 마감일을 정의하면 특정 기간 내에만 문서를 보관용 계정에 업로드할 수 있습니다. 시작 날짜나 마감일 또는 둘 다를 지정하십시오.

**첨부 파일:** 첨부 파일 주제 작성자는 필드에서 파일을 업로드할 수 있습니다. 여러 파일을 단일 ZIP 파일로 업로드할 수 있습니다.

**주제 선택/선택 해제 시 이메일 알림:** 이 옵션을 선택하면 코스 참가자가 주제를 선택하거나 선택 취소하는 경우 이메일 알림을 받게 됩니다.

![Topic_Assignment_EN](/img/course_elements/Topic_Assignment_EN.png)

"주제 편집"을 통해 편집 모드로 이동합니다.

주제 할당에서 주제를 삭제하려면 "주제 삭제"를 클릭하십시오.

더 이상 참가자가 주제를 선택할 수 없어야 하는 경우 "채움"에서 주제 설정 상태"를 선택하십시오. "주제 상태를 "공석"으로 재설정"을 통해 이미 등록되어 수락된 참가자가 있더라도 주제를 새로 열 수 있습니다. 마지막 두 개의 버튼은 코스 작성자가 참가자를 수동으로 수락하는 옵션과 함께 주제 할당을 제공한 경우에만 표시됩니다.

"폴더" 및 "참가자 관리" 탭

### **참가자 관리 방법**

주제 지정 구성에서 주제 작성자가 코스 참가자를 수락해야 하는 경우 누군가가 귀하의 주제에 지원하는 즉시 표에 "참가자 확인"이라는 메모가 표시됩니다.

![Topic_Assignement_TN_EN](/img/course_elements/Topic_Assignement_TN_EN.png)

![Topic_Assignement_TN2_EN](/img/course_elements/Topic_Assignement_TN2_EN.png)

이제 "주제 할당" 탭을 열고 후보자의 지원을 수락하십시오.

후보자는 귀하의 주제에 지원하는 코스 참가자입니다. "다음으로 참가자 수락"을 통해 주제를 누구에게 할당할지 결정할 수 있습니다. 수락된 모든 참가자는 "참가 수락" 목록에 추가되며 원하는 경우 이메일을 통해 알림을 받을 수 있습니다. 수락하지 않는 후보자를 강조 표시하고 "삭제"를 클릭하십시오. 원하는 경우 해당 후보자에게도 이메일로 통지됩니다.

공석 수를 제한하지 않은 경우 이 절차를 여러 번 반복할 수 있습니다. 주제에 대한 추가 적용을 피하기 위해 "설명" 탭에서 "주제 설정 상태"를 "채움"으로 선택하십시오.

이 탭의 참가자와 추가 주제 관리자를 수동으로 추가하거나 제거할 수도 있습니다. 참가자는 주제를 편집할 수 없습니다.

### **파일 업로드 및 반환 방법**

"폴더" 탭, "드롭 상자" 섹션에서 코스 참가자가 제출한 모든 파일을 찾을 수 있습니다. "반환 상자"섹션에서 이미 수정 된 파일을 넣을 수 있습니다. 각 코스 참가자에 대해 하나의 하위 폴더가 있습니다.

**사용자의 관점에서:**

주제 상태가 "무료"로 설정된 경우 사용자는 가능한 최대 주제 선택을 초과하지 않는 한 주제에 등록할 수 있습니다. 주제 상태가 "점유됨"으로 설정되면 더 이상 사용자를 등록할 수 없습니다. 이미 주제를 선택한 경우 주제 상태는 주제 담당자가 귀하를 참가자로 수락해야 하는 경우 "임시 할당됨"이고 등록이 자동인 경우 "할당됨"입니다. 주제 소유자가 귀하를 참가자로 수락하면 주제 상태가 "확실히 할당됨"으로 설정됩니다.

## 코스 요소: 링크 목록

![linklist](/img/course_elements/linklist.png)

코스 요소 "링크 목록"을 통해 작성자는 코스와 관련된 링크 모음을 신속하게 조합할 수 있습니다. HTML 능숙도가 필요하지 않습니다. 코스 편집기를 열고 링크 목록 코스 요소로 이동한 다음 "구성" 탭을 열고 링크로 추가하려는 웹사이트의 URL을 입력하거나 돋보기 아이콘을 클릭하여 대상 파일을 선택하기만 하면 됩니다. 이제 열려 있는 모달 창에서 파일을 업로드할 수 있습니다. 그런 다음 링크를 새 창에서 열 것인지 아니면 같은 창에서 열 것인지 선택하고 링크 제목을 입력합니다. 링크에 대한 설명이나 기타 추가 정보는 주소 필드 아래에 있는 설명 필드를 통해 추가할 수 있습니다. 휴지통 / + 버튼을 사용하여 링크를 제거하거나 추가합니다.

![Linklist_EN](/img/course_elements/Linklist_EN.png)

![Linklist_output_EN](/img/course_elements/Linklist_output_EN.png)

## 코스 요소 "날짜 지정"

![dateentry](/img/course_elements/dateentry.png)

여기에서 사용자가 등록할 수 있는 날짜를 만들고 편집할 수 있습니다. 등록 취소가 허용되는지 여부도 정의할 수 있습니다. 또한 참가자를 관리할 수 있습니다.

날짜 할당은 "구성" 탭의 코스 편집기와 편집기가 닫힐 때 설정할 수 있습니다.