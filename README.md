한국어 · [English](README.en.md)

# Junha Kang

보안 실무자이자 독립 연구자입니다. 직접 띄운 모델로 도는 에이전트 실행기를 만들고, 그 실행기의 성능을 어떻게 측정해야 하는지 살펴보았습니다.

## stewart

**직접 띄운 모델에게 작업 폴더를 맡기는 작은 에이전트 실행기** · [저장소](https://github.com/midopa-dept/stewart)

[![stewart 허브: 결제 금액 버그를 재현하고 고치는 대화](https://github.com/midopa-dept/stewart/raw/main/docs/images/hero.png)](https://github.com/midopa-dept/stewart/blob/main/docs/demo.md)

- 어떤 OpenAI 호환 서버(llama.cpp, vLLM)나 Anthropic Messages API 에도 붙습니다.
- 브라우저 허브(여러 대화·갈래·작업자)와 터미널(`stewart chat`)로 씁니다.
- 바깥 API 로 도는 허브는 이름별 인스턴스로 따로 띄워 설정·상태·기억을 가르고, macOS 샌드박스 안에서 돌립니다.
- 작업 폴더 경계와 승인, 기억과 스킬, 두 단계 문맥 압축(오래된 도구 결과 가리기, 그다음 요약)이 있습니다.
- 같은 Claude 모델로 같은 과제를 풀 때 Claude Code 보다 회당 비용 0.69–0.77배, 걸린 시간 0.72–0.80배를 썼고 성공률은 가를 만한 차이가 없었습니다. 자체 과제 16개로 한 탐색 측정이라 일반 성능으로 읽으면 안 됩니다.

[README](https://github.com/midopa-dept/stewart#readme) · [데모 화면](https://github.com/midopa-dept/stewart/blob/main/docs/demo.md) · [참고 연구 노트](https://github.com/midopa-dept/stewart/blob/main/docs/research-notes.md)

짝 도구 [stewart-cloud](https://github.com/midopa-dept/stewart-cloud)(v0.2.1): Vast.ai 에서 빌린 GPU 에 vLLM 으로 열린 모델을 띄우고, 내 Tailscale 망에서만 닿게 해 stewart 에 붙입니다.

## 최근 관심사

- 작은·로컬 모델을 위한 실행기 설계: 모델이 약한 곳을 실행기 쪽 장치로 받치기
- 실행기를 재는 방법: 미리 적어 둔 계획(사전 등록), 기준선, 같은 모델로 나란히 재기
- 자기 기록에서 배워 나아지는 에이전트: 실행 기록에서 배우기와 미세조정(진행 중)
- 셸을 돌리는 에이전트의 안전장치와 격리
- 폐쇄망 PC 에서 로컬 LLM 을 쓰는 교육(공개 교재 local-ai-textbook)

## 그 밖의 저장소

- [cairn-harness](https://github.com/midopa-dept/cairn-harness): LLM 에이전트가 오래 코드를 바꾸는 프로젝트를 위한 소형 선언형 계약(권한, 작업 상태, 확인과 수락, 근거, 중단 뒤 복구). 릴리스 후보 `1.0.0-candidate.5`.
- [agent-workspace-hardening](https://github.com/midopa-dept/agent-workspace-hardening): 개인 Mac 에서 코딩 에이전트가 닿는 범위를 줄이는 관리 설정과 git-guard 훅, 그리고 권한 규칙이 생각대로 돌지 않은 곳을 찾은 시험 기록.
- [education-harness](https://github.com/midopa-dept/education-harness): 코딩 에이전트와 교육자료를 만들며 얻은 공통 규칙. 인터넷 없는 PC 에서 로컬 LLM 을 실습하는 2일 과정 하나를 끝까지 만들며 나왔습니다.
- [local-ai-textbook](https://github.com/midopa-dept/local-ai-textbook): 그 과정의 교과서(한국어, 161쪽). 내 PC 안에서 도는 작은 모델로 실습하며 AI 의 답을 원본 자료와 대조하는 법을 배웁니다.
- [ai-knowledge-atlas](https://github.com/midopa-dept/ai-knowledge-atlas): 한국어 비선형 AI 교재의 지식 그래프(개념 504개, 학습목표 817개)와 검증기, 그리고 검토 후보인 첫 장(Attention 과 Transformer).

문서는 대부분 한국어입니다. local-ai-textbook 밖의 저장소에는 영어 README 가 있습니다.

ORCID: https://orcid.org/0009-0006-9062-8353