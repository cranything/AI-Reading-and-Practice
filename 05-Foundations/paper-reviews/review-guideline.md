# 논문 리뷰 가이드라인 (Paper Review Guideline)

<br>

## 1. 저자의 GitHub 및 코드 활용 확인 (Check Author’s GitHub Repository)

### 구체화

- 논문에서 제시된 방법이 실제 구현되어 있는지 확인
- GitHub 코드로부터 모델 구조, 전처리, 학습 방식 등을 파악
- 코드 실행 및 실험 재현(reproduce) 또는 개선

<br>

## 2. 논문이 소개하는 핵심 방법 정리 (Understand the Main Method)

### 구체화

- 논문의 목적(Objective)과 제안 기법(Proposed Method) 요약
- 해결하고자 하는 문제와 아이디어 정리
- 구조도, 알고리즘 흐름도, 수식 요약 등 포함

<br>

## 3. 배경지식 및 기초 개념 정리 (Background and Preliminaries)

### 구체화

- 전제하고 있는 기본 개념(CNN, Self-Attention, KL-Divergence 등) 정리
- 수식이나 기호에 대한 해설 포함
- 관련 논문 또는 방법론 간단 요약

<br>

## 4. 기존 방법들과의 비교 (Comparison with Baseline Methods)

### 구체화

- 기존 방법들과 비교하여 성능 또는 구조적 이점을 명확히 기술
- 정확도, 연산량, 일반화 성능 등의 비교
- 표 또는 그래프를 활용한 시각적 비교

<br>

## 5. 실험 결과 분석 (Experimental Result Analysis)

### 구체화

- 수치를 단순 나열하지 않고 결과를 해석
- Ablation Study, Hyperparameter Tuning 결과 분석 포함
- 실패 사례(failure cases), 한계점 등도 기술

<br>

## 6. 다양한 Task에 대한 성능 (Generalization to Multiple Tasks)

### 구체화

- 분류, 검출, 세분화 등 여러 task에 적용된 결과 제시
- 실제 응용 가능성 및 도메인 적응 여부 분석
- 처리 속도, 연산 자원 요구 등도 함께 고려

<br>

## 전체 정리 요약 (Review Summary Table)

| 항목               | 주요 내용                         | 확인할 포인트                |
|--------------------|----------------------------------|-------------------------------|
| 저자 GitHub        | 코드 공개 여부                    | 재현 가능한가?                |
| 핵심 방법          | 제안된 방법의 구조                | 기존 방법과 차이점은?         |
| 배경 지식          | 전제 개념 이해                    | 기초 용어, 수식 이해          |
| 기존 비교          | Baseline과 비교 실험              | 어떤 점에서 더 나은가?        |
| 실험 분석          | 성능 향상 요인 분석               | ablation, 분석적 해석         |
| 다양한 태스크      | 다중 태스크 적용 가능성           | 범용성, 확장성 확인           |

<br>

## LaTeX 템플릿 예시

```latex
\documentclass[11pt]{article}
\usepackage[a4paper, margin=1in]{geometry}
\usepackage{amsmath, amssymb}
\usepackage{graphicx}
\usepackage{hyperref}
\usepackage{enumitem}
\usepackage{kotex} % 한글 사용 시 필요

\title{논문 리뷰: \textbf{[논문 제목 작성]}}
\author{리뷰어: [이름]}
\date{\today}

\begin{document}
\maketitle

\section*{1. 논문 기본 정보}
\begin{itemize}[leftmargin=1.5em]
  \item \textbf{제목}: [논문 제목]
  \item \textbf{저자}: [저자명]
  \item \textbf{학회/저널}: [예: CVPR 2024]
  \item \textbf{링크}: \url{https://arxiv.org/abs/xxxx.xxxxx}
  \item \textbf{GitHub}: \url{https://github.com/author/project}
\end{itemize}

\section*{2. 논문 개요 (Summary)}
[논문이 해결하려는 문제와 주요 기여를 간략히 정리합니다.]

\section*{3. 제안 방법 (Proposed Method)}
[모델 구조, 주요 알고리즘, 수식 요약 등을 포함합니다.]

\section*{4. 배경 지식 (Background)}
[논문을 이해하기 위해 필요한 전제 지식, 관련 용어 정리 등.]

\section*{5. 기존 방법과의 비교 (Comparison with Prior Work)}
[성능, 구조, 효율성 등의 측면에서 비교 분석합니다.]

\section*{6. 실험 결과 분석 (Experiments and Analysis)}
\begin{itemize}
  \item \textbf{Dataset}: 사용된 데이터셋 이름과 특성
  \item \textbf{Metric}: 정확도, F1-score 등 성능 지표
  \item \textbf{Ablation}: 구성요소 별 성능 변화
  \item \textbf{Failure case}: 한계나 실패 사례
\end{itemize}

\section*{7. 다양한 태스크에 대한 적용 (Multi-task Generalization)}
[제안된 방법이 다양한 task에 어떻게 적용되었는지 기술합니다.]

\section*{8. 한계 및 향후 과제 (Limitations and Future Work)}
[논문에서 언급된 한계와 연구자의 제안 방향 또는 본인의 생각.]

\section*{9. 요약 및 총평 (Summary and Comments)}
[논문의 의의, 실무 적용 가능성, 개인적인 인사이트 등을 정리.]

\end{document}
```

<br>

## 사용 방법

### Overleaf 사용

1. [https://www.overleaf.com](https://www.overleaf.com) 접속
2. "Blank Project" 생성
3. 위 LaTeX 템플릿 코드 붙여넣기
4. Compile 클릭

### 로컬 사용

- `.tex` 확장자로 저장
- TeX Live, MiKTeX 등을 설치 후 `pdflatex 파일명.tex`으로 컴파일