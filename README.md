# Has-Entrance-Examination-System

하나고등학교의 동아리 입시 시스템을 만들기 위한 단체입니다.

현재 하나고등학교의 동아리 입시 시스템을 보면 매우 복잡하며 불편합니다. 이 시스템은 이를 개선하기 위해 만들어진 시스템입니다.

1. 편리한 지원 및 확인 과정: 현재의 동아리 지원은 메일을 통해 이루어지고 있어서 지원서를 정리하고 지원을 확인하는 과정에서 불편함이 있습니다. 통합 시스템을 통해 지원자들은 편리하게 지원서를 제출하고 동아리 입시 과정을 확인할 수 있게 됩니다.
2. 개인정보 보호: 현재의 동아리 지원 방식은 개인 번호를 공개해야 하기 때문에 개인정보 보호에 취약합니다. 통합 시스템을 통해 개인정보를 안전하게 관리하고 처리함으로써 개인정보 문제를 사전에 방지할 수 있습니다.
3. 공정성 확보: 동아리 결과 통보 시 동아리장과 합격 및 불합격자간에 문자를 주고 받는 것은 공정성과 학우 간 신뢰를 해치는 요소가 될 수 있습니다. 통합 시스템을 통해 면접 관련 사항과 결과를 투명하게 전달함으로써 공정성을 높이고 동아리 간의 갈등을 예방할 수 있습니다.

## 팀원
| 이름 | 깃험 | 역할 |
|------|------|------|
|안호성|||

## Todo
### 구현 완료된 기능
- [x] ~~회원가입, 로그인~~
  - [x] ~~회원가입~~: 필요한 정보(이름, 인트라넷 ID/PW, 사이트 ID/PW, 이메일 주소 등)를 입력하여 회원가입을 완료
  - [x] ~~인트라넷 로그인으로 인증~~
  - [x] ~~학생 구분(동장, 신입생)~~
- [x] ~~신입생~~
  - [x] ~~동아리 지원~~: 신입생은 지원하고자 하는 동아리를 선택하여 지원할 수 있습니다.
  - [x] ~~동아리 지원 취소~~: 신입생은 이미 지원한 동아리 지원을 취소할 수 있습니다.
  - [x] ~~지원 동아리 확인~~: 신입생은 자신이 지원한 동아리 목록을 확인할 수 있습니다.
  - [x] ~~합불 여부 확인~~: 신입생은 자신이 지원한 동아리의 합불 여부를 확인할 수 있습니다.
  - [x] ~~면접 장소 확인~~: 신입생은 자신의 면접 장소를 확인할 수 있습니다.
  - [x] ~~면접시간 확인~~: 신입생은 자신의 면접 시간을 확인할 수 있습니다.
  - [x] ~~지원서 제출~~: 신입생은 지원서를 작성하여 해당 동아리에 제출할 수 있습니다.
  - [x] ~~피드백 확인~~: 면접 후 신입생은 면접 결과와 피드백을 확인할 수 있습니다.
- [x] ~~동장~~
  - [x] ~~동아리 지원자 불러오기~~: 동아리장은 자신의 동아리에 지원한 지원자 목록을 불러올 수 있습니다.
  - [x] ~~신입생 합/불 지정~~: 동아리장은 지원자들에 대해 합격 또는 불합격 여부를 지정할 수 있습니다.
  - [x] ~~면접 장소 지정~~: 동아리장은 면접을 진행할 장소를 지정할 수 있습니다.
  - [x] ~~면접 시간 안내~~: 동아리장은 면접 일정과 시간을 지원자들에게 안내할 수 있습니다.
  - [x] ~~지원서 화인~~: 동아리장은 지원자들의 지원서 내용을 확인할 수 있습니다.
  - [x] ~~신입생 피드백 전달~~: 면접 후 동아리장은 지원자들에게 면접 결과와 피드백을 markdown으로 전달할 수 있습니다.

### 개선 예정 사항
- [ ] 기술적 개선
  - [ ] React로 Frontend 추가 개발
  - [ ] Postgresql로 마이그레이견
  - [ ] DB pooling 도입(Psycopg)
  - [ ] Svelte 애니메이션 추가
  - [ ] 코드 주석 제거
  - [ ] Response Model 없는 router에 Model 추가
- [ ] 기능 개선
  - [ ] 기존 체계에 맞게 한 차수당 동아리 2개 지원 가능하도록 수정
    - [ ] 한 차수내 면접 시간 충돌 대비
  - [ ] 최종 동아리 확정 기능 추가
  - [ ] *(관리자 계정 추가)* - SQL 외부 연결로 대체 가능.
  - [ ] 동아리원 개정 추가
  - [ ] 동아리 취소 절차 개선
  - [ ] 세부적 일정 지원
    - [ ] 지원서 제출 기한
    - [ ] 지원 가능 시간
    - [ ] 면접 결과 확인 가능 시간
  - [ ] 동아리 홍보물 개시
  - [ ] ~~지원 전 동아리 Q&A~~

## 개발 환경

* Python 3.10.11
* FastAPI 0.95.1
```
pip install -r requirements.txt
```
* nodejs V18.16.0
* svelte@3.59.0
* VITE v4.3.5
```
cd HasEntranceExaminationSystem/frontend/
npm install
```

## 실행

* FastAPI
```
cd HasEntranceExaminationSystem/
uvicorn main:app --reload
```
* Svelte

```
cd HasEntranceExaminationSystem/frontend/
npm run dev
```
---
# 개인 레포지토리 깃 로그

[깃 로그](https://github.com/BetaTester772/HasEntranceExaminationSystem-Public/blob/master/git-log.txt)
---
login_proc.py from [here](https://github.com/BetaTester772/ExamVenueInquirySystem/blob/main/login_proc.py)
