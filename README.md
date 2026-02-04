# RAG Study & Persona-based Requirements Discovery

이 저장소는 RAG(Retrieval-Augmented Generation) 학습 과정과  
LLM을 활용한 페르소나 기반 인터뷰를 통해 요구사항을 도출하는 실험 코드를 정리한 개인 학습 리포입니다.

이론 정리보다는 직접 구현하고 실험한 코드 위주로 구성되어 있습니다.

---

## RAG 학습 노트북

RAG의 핵심 구성 요소를 단계별로 실습하며 정리했습니다.

- `RAG-Chapter01.ipynb`
- `RAG-Chapter02.ipynb`
- `RAG-Chapter03.ipynb`
- `RAG-Chapter04.ipynb`
- `RAG-Chapter05.ipynb`
- `RAG-Chapter06.ipynb`
- `RAG-Chapter08.ipynb`
- `RAG-Chapter09.ipynb`

각 노트북에는 다음과 같은 내용을 포함합니다.

- RAG 기본 개념
- 문서 청킹 및 임베딩
- 검색(Retrieval) 전략
- 검색 결과와 LLM 결합
- 간단한 실험 및 코드 예제

---

## 페르소나 기반 요구사항 도출 실험

### `persona_interview_chain.ipynb`

사용자 요청을 입력으로 받아  
다수의 페르소나를 생성하고 인터뷰를 수행한 뒤,  
이를 체이닝하여 요구사항 정의로 확장할 수 있는 구조를 실험한 코드입니다.

### 주요 흐름

1. 사용자 요청 기반 다중 페르소나 생성
2. 페르소나별 인터뷰 질문 생성
3. 페르소나 관점의 응답 생성
4. 인터뷰 결과 누적 및 상태 관리
5. 반복을 통한 요구사항 정제 가능 구조

### 사용 기술

- Pydantic (상태 및 데이터 모델 정의)
- LangChain
- OpenAI Chat Model
- 체이닝 기반 워크플로우 설계

---

## 목적

- RAG 구조에 대한 이해 심화
- LLM 체이닝 패턴 실습
- 사용자 요구사항 정의 자동화 가능성 탐색
- 실무 적용 전 단계의 실험 코드 축적

---

## 참고

- 개인 학습 및 실험 목적의 코드입니다.
- 구조는 추후 리팩터링 및 모듈화될 수 있습니다.
