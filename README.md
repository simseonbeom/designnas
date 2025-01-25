


## 디자인나스 웹 프로그래밍 저장소

---

기초 웹 프로그래밍에 필요한 내용들을 순서대로 학습합니다.



- [x] 환경설정
- [x] HTML 기본 태그와 사용방법



| **타입 (`type`)** | **설명**                                                                 | **사용 예제 코드**                                                                                   | **주요 속성 및 특징**                                                                                     |
|------------------|---------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| `text`          | 일반적인 텍스트 입력 필드                                                    | `<input type="text" placeholder="이름 입력" />`                                                | - `maxlength`, `placeholder`, `value` 등 사용 가능<br>- 기본값으로 글자 입력 가능                                |
| `password`      | 비밀번호 입력 (입력값이 화면에 표시되지 않고 ● 또는 ●●●로 표시됨)                   | `<input type="password" placeholder="비밀번호 입력" />`                                        | - 입력값 보호<br>- 브라우저 자동완성 기능 동작                                                      |
| `email`         | 이메일 형식 입력 필드                                                       | `<input type="email" placeholder="example@example.com" />`                                    | - 이메일 형식 유효성 검사 가능 (`@` 포함 여부 등)<br>- 모바일 키보드에서 "@" 버튼 표시                          |
| `number`        | 숫자 입력 필드                                                          | `<input type="number" min="0" max="100" step="5" />`                                          | - 숫자만 입력 가능<br>- `min`, `max`, `step` 속성을 활용해 범위와 간격 설정 가능                                 |
| `tel`           | 전화번호 입력 필드                                                        | `<input type="tel" placeholder="전화번호 입력" />`                                             | - 전화번호 형식 유효성 검사는 브라우저에 따라 다름<br>- 모바일에서 숫자 키패드 자동 표시                            |
| `url`           | URL(웹 주소) 입력 필드                                                   | `<input type="url" placeholder="https://example.com" />`                                      | - URL 형식 유효성 검사 가능<br>- `https://`로 시작하는 값 요구                                      |
| `search`        | 검색 필드                                                             | `<input type="search" placeholder="검색어 입력" />`                                           | - 검색 UI 최적화<br>- 일부 브라우저에서 기본 검색 버튼 제공                                           |
| `file`          | 파일 업로드 필드                                                        | `<input type="file" />`                                                                      | - 파일 선택 다이얼로그 표시<br>- `accept` 속성으로 파일 형식 제한 가능 (예: `accept="image/*"`)                      |
| `checkbox`      | 다중 선택(체크박스)                                                     | `<input type="checkbox" id="check1" /><label for="check1">옵션1</label>`                      | - 여러 값을 동시에 선택 가능<br>- 상태 확인: `checked` 속성 사용                                      |
| `radio`         | 단일 선택(라디오 버튼)                                                   | `<input type="radio" name="group1" id="option1" /><label for="option1">옵션1</label>`         | - 같은 `name` 속성을 가진 그룹에서 하나만 선택 가능<br>- 상태 확인: `checked` 속성 사용                            |
| `range`         | 슬라이더를 사용해 값 입력                                                  | `<input type="range" min="0" max="100" step="1" />`                                           | - 범위와 간격(`min`, `max`, `step`) 설정 가능<br>- 기본적으로 숫자가 아닌 슬라이더 형태 제공                            |
| `color`         | 색상 선택 필드                                                         | `<input type="color" />`                                                                     | - 색상 선택기를 표시<br>- 기본 색상 값: `value` 속성 사용                                            |
| `date`          | 날짜 선택 필드                                                         | `<input type="date" />`                                                                      | - 날짜 선택 위젯 제공<br>- 날짜 형식은 `YYYY-MM-DD`                                                 |
| `time`          | 시간 선택 필드                                                         | `<input type="time" />`                                                                      | - 시간 선택 위젯 제공<br>- 시간 형식은 `HH:MM`                                                    |
| `datetime-local`| 날짜 및 시간 선택 필드                                                     | `<input type="datetime-local" />`                                                           | - 날짜와 시간을 함께 선택 가능<br>- 로컬 시간대 기준                                                 |
| `month`         | 월 선택 필드                                                          | `<input type="month" />`                                                                     | - 월 및 연도 선택<br>- 형식: `YYYY-MM`                                                            |
| `week`          | 주 단위 선택 필드                                                       | `<input type="week" />`                                                                      | - 주 및 연도 선택<br>- 형식: `YYYY-W##` (예: 2025-W04)                                             |
| `hidden`        | 숨겨진 입력 필드                                                        | `<input type="hidden" name="userID" value="12345" />`                                         | - 사용자에게 표시되지 않지만 데이터를 폼에 포함 가능                                                |
| `button`        | 클릭 가능한 버튼                                                        | `<input type="button" value="클릭하세요" />`                                                  | - 클릭 이벤트는 반드시 자바스크립트로 처리해야 동작                                                 |
| `submit`        | 폼 전송 버튼                                                          | `<input type="submit" value="전송" />`                                                      | - 클릭 시 폼 데이터를 서버로 전송<br>- 기본적으로 폼 제출 동작 수행                                    |
| `reset`         | 폼 리셋 버튼                                                          | `<input type="reset" value="초기화" />`                                                     | - 폼의 입력 값을 초기 상태로 되돌림                                                            |



