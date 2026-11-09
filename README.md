# QFF 2026 — Q-LINK

[한국어 안내](#한국어-안내) · [English guide](#english-guide)

## 한국어 안내

**Qiskit Fall Fest · QUICK · 고려대학교 | 참가자용**

Alice, Bob, Charlie의 세 실험실을 연결하는 양자 네트워크 실험에 참여하세요. 측정과 얽힘 자원을 점검하고, 양자 텔레포테이션으로 상태를 전송한 뒤, GHZ–Mermin 게임에서 세 실험실의 협력 성능을 확인합니다.

### 언어 선택 · Choose your language

| 언어 / Language | Google Colab | 노트북 파일 / Notebook | 사용 안내 / Guide |
|---|---|---|---|
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [한국어 안내](#한국어-안내) |
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [English guide](#english-guide) |

**English participants:** Open the English notebook above and follow the [English guide](#english-guide). The notebook selects English grading feedback automatically.

두 언어의 **문제·구성·배점·채점 기준은 동일**합니다. 각 노트북은 해당 언어의 채점 피드백과 제출 안내를 자동으로 표시하므로 언어 설정 코드를 수정할 필요가 없습니다.

문제 설명, 이미지, 실험 코드와 채점 도구 설치 셀이 모두 **선택한 노트북 하나에 들어 있습니다.** 내려받으려면 노트북 파일 화면의 **Download raw file** 버튼을 누르세요. 같은 파일을 Colab·VS Code·Jupyter에서 사용할 수 있습니다.

### 시작하기

1. Colab에서 열었다면 **자신의 사본으로 저장**하세요. VS Code·Jupyter에서는 내려받은 `.ipynb`를 여세요.
2. Colab에서는 **CPU 런타임**, VS Code·Jupyter에서는 **Python 3.10–3.13 커널**을 사용하세요. 로컬 환경은 **Python 3.12**를 권장합니다.
3. **준비 A 셀만 먼저 실행**하세요. [Grader 2.0.6](https://github.com/equivoque-jk/qff-2026-grader/releases/tag/v2.0.6)과 필요한 실험 도구가 설치됩니다. 최초 설치에는 인터넷 연결이 필요합니다.
4. 재시작 안내가 나오면 Colab에서는 **런타임 → 세션 다시 시작**, VS Code·Jupyter에서는 **커널 재시작**을 선택한 뒤 준비 A를 다시 실행하세요.
5. 준비 완료를 확인한 뒤 준비 B·C·D와 해당 문제의 제공 도구·문제 셀을 순서대로 실행하세요.

### 문제 구성

| 구분 | 내용 | 배점 |
|---|---|---:|
| 1. 측정과 얽힘 | 측정 기저에 따른 상태 구별과 Bell·GHZ 자원 준비 | 30점 |
| 2. 양자 텔레포테이션 | 고장 회로 진단, 전송 회로 복구와 검증 | 40점 |
| 3. GHZ–Mermin 게임 | 고전 전략과 양자 전략의 승률 비교 | 30점 |
| 선택 2-5 | 두 큐비트의 전체 상태 전송 | 추가 12점 |
| 선택 3-5 | 위상 오류가 있는 자원의 게임 성능 분석 | 추가 8점 |

기본 **14문항은 100점**, 선택 **2문항은 추가 20점**입니다. 선택 문항은 원하는 문제만 풀 수 있으며, 풀지 않아도 기본 문항 점수에는 영향을 주지 않습니다.

### 풀이 방법

- 답안 함수의 **`TODO BEGIN`과 `TODO END` 사이**에 코드를 작성하세요. 해당 영역의 `raise NotImplementedError(...)`를 지우고 자신의 구현으로 교체하세요.
- 함수 선언, 제공된 초기화 코드, 마지막 `return`, 실행·채점 셀은 그대로 두세요. 답안 함수는 선택 문항을 포함해 총 23개입니다.
- 각 문항의 **반환 형식과 채점 사항**을 확인하세요. 수치 답안에는 표본 실험의 추정치를 복사하지 말고, 문제에서 요구하는 정확한 값을 계산해 반환하세요.
- 실험 메모에는 계산 과정과 결과를 해석한 내용을 적으세요. 실험 메모와 마지막 개통 보고서는 채점 대상이 아닙니다.

**2-1과 선택 2-5에서 제공된 고장 회로의 실패 메시지는 의도된 결과입니다.** 메시지를 단서로 결함을 찾고, 수정한 회로가 검증을 통과하는지 확인하세요.

### 채점 및 제출

1. 답안을 저장한 뒤 Colab에서는 **런타임 → 모두 실행**, VS Code·Jupyter에서는 **Run All**을 선택하세요. 작성하지 않은 선택 문항의 TODO는 그대로 두세요.
2. 마지막 셀에서 **기본·추가 점수와 미완성·오류 항목**을 확인하세요. 문제별 실험 출력과 답안 함수의 반환값 검사는 다르므로 마지막 채점 결과도 확인해야 합니다.
3. 아래 방법으로 **제출 ZIP**을 저장하고, **풀이를 작성한 노트북도 `.ipynb`로 별도 저장**하세요. 노트북은 제출 ZIP에 포함되지 않습니다. Colab에서는 런타임을 종료하기 전에 두 파일을 내려받으세요.
4. **제출 ZIP과 작성한 `.ipynb` 두 파일을 행사에서 안내한 제출처에 함께 제출**하세요.

| 실행 환경 | 제출 ZIP 저장 | 작성한 노트북 저장 |
|---|---|---|
| Colab | 마지막 셀이 브라우저에 자동 다운로드를 요청합니다. | **파일 → 다운로드 → .ipynb 다운로드** |
| Jupyter | 새로 실행한 마지막 셀의 **제출 ZIP 다운로드** 링크를 누르세요. | 노트북을 저장하세요. |
| VS Code | 마지막 셀의 **제출 ZIP:** 옆 경로에 로컬 파일로 저장됩니다. | 노트북 파일을 저장하세요. |

답안을 수정하고 다시 모두 실행하면 새 실행 ID로 결과가 저장됩니다. **마지막 채점 결과의 실행 ID와 제출 ZIP이 일치하는지 확인**하세요. 채점 셀 실행과 파일 저장만으로 제출이 접수되지는 않습니다.

**제출은 개인 단위로 진행합니다.** 작성한 노트북은 **`학번_이름.ipynb`**로 저장해 제출 ZIP과 함께 제출하세요.

**마감 날짜·시각, 제출 폼·업로드 링크, 문의 채널은 행사 당일 공지에 따릅니다.**

### 실행 중 문제가 생겼다면

- **설치가 실패할 때:** 준비 A의 오류 메시지와 인터넷 연결을 확인한 뒤 다시 실행하세요.
- **세션이나 커널을 재시작했을 때:** 화면에 예전 출력이 남아 있어도 변수와 함수 정의는 사라집니다. 준비 A부터 필요한 셀을 순서대로 다시 실행하세요.
- **Colab 자동 다운로드가 시작되지 않을 때:** 마지막 셀에 표시된 저장 경로를 확인하고, Colab 왼쪽 파일 패널에서 해당 ZIP을 다운로드하세요.
- **Jupyter에서 저장된 예전 출력의 링크를 사용할 때:** 문제지를 모두 실행한 뒤, 마지막 셀에 새로 표시된 다운로드 링크를 누르세요.

해결되지 않는 문제가 생기면 행사에서 안내한 문의 채널로 오류 메시지와 해당 셀을 운영진에게 보여 주세요. 자세한 문항별 조건은 문제지를, 채점 기준은 [배점표](https://github.com/equivoque-jk/qff-2026-grader/blob/main/docs/SCORING.md)를 확인하세요.

---

## English Guide

**Qiskit Fall Fest · QUICK · Korea University | Participant Edition**

Join a quantum network experiment connecting the laboratories of Alice, Bob, and Charlie. Inspect measurement equipment and entanglement resources, transfer a quantum state by teleportation, and evaluate how the three laboratories cooperate in the GHZ–Mermin game.

### Choose your language

| Language | Google Colab | Notebook file | Guide |
|---|---|---|---|
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | This section |
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [한국어 안내](#한국어-안내) |

Both editions have **the same exercises, structure, point allocation, and grading criteria**. Each notebook automatically selects its language for grading feedback and submission instructions; you do not need to edit any language settings.

**The notebook you choose contains all exercise descriptions, figures, experiment code, and the grader installation cell.** To download it, open the notebook file page and select **Download raw file**. The same file works in Colab, VS Code, and Jupyter.

### Getting started

1. If you open the notebook in Colab, **save your own copy**. In VS Code or Jupyter, open the downloaded `.ipynb` file.
2. Use a **CPU runtime** in Colab or a **Python 3.10–3.13 kernel** in VS Code or Jupyter. **Python 3.12** is recommended for local use.
3. **Run only Setup A first.** It installs [Grader 2.0.6](https://github.com/equivoque-jk/qff-2026-grader/releases/tag/v2.0.6) and the tools required for the experiments. An internet connection is required for the initial installation.
4. If prompted to restart, select **Runtime → Restart session** in Colab, or **restart the kernel** in VS Code or Jupyter. Then run Setup A again.
5. Once setup is complete, run Setup B, C, and D, followed by the provided tools and exercise cells in order.

### Exercise structure

| Part | Content | Points |
|---|---|---:|
| 1. Measurement and Entanglement | Distinguish states through measurement bases and prepare Bell and GHZ resources | 30 |
| 2. Quantum Teleportation | Diagnose, repair, and verify a faulty teleportation circuit | 40 |
| 3. GHZ–Mermin Game | Compare the winning probabilities of classical and quantum strategies | 30 |
| Optional 2-5 | Transfer the full state of two qubits | 12 additional |
| Optional 3-5 | Analyze game performance with phase errors in the shared resource | 8 additional |

The **14 core exercises are worth 100 points**, and the **two optional exercises offer 20 additional points**. You may complete either or both optional exercises. Leaving them unanswered does not affect your core score.

### Completing the exercises

- Write your code **between `TODO BEGIN` and `TODO END`** in each answer function. Remove the `raise NotImplementedError(...)` statement in that region and replace it with your implementation.
- Preserve function signatures, provided initialization code, final `return` statements, and the execution and grading cells. There are 23 answer functions, including the optional exercises.
- Read each exercise's **return format and grading criteria**. Numerical answers must return the exact values requested in the exercise; do not copy estimates from sampling experiments.
- Use the Experiment Notes to record your calculations and interpret the results. The notes and the final Network Commissioning Report are not graded.

**The failure messages from the provided faulty circuits in 2-1 and optional 2-5 are intentional.** Use them to identify the defects, then verify that your repaired circuits pass the checks.

### Grading and submission

1. Save your answers, then select **Runtime → Run all** in Colab or **Run All** in VS Code or Jupyter. Leave the TODOs unchanged for optional exercises you have not attempted.
2. In the final cell, check your **core and additional scores, incomplete items, and errors**. Experiment outputs and checks of answer-function return values serve different purposes, so always inspect the final grading result.
3. Save the **submission ZIP** as described below, and **save the completed notebook separately as an `.ipynb` file**. The notebook is not included in the ZIP. In Colab, download both files before ending the runtime.
4. **Submit both the ZIP and your completed `.ipynb` to the destination announced by the event organizers.**

| Environment | Save the submission ZIP | Save your completed notebook |
|---|---|---|
| Colab | The final cell requests an automatic browser download. | **File → Download → Download .ipynb** |
| Jupyter | Click **Download submission ZIP** in the output of the newly executed final cell. | Save the notebook. |
| VS Code | The ZIP is saved locally at the path displayed after **Submission ZIP:** in the final cell. | Save the notebook file. |

After editing your answers and running all cells again, the results are saved under a new run ID. **Check that the run ID in the final grading result matches the submission ZIP.** Running the grading cell and saving files does not by itself submit your work.

**Submissions are individual.** Name your completed notebook **`학번_이름.ipynb`** (student ID and name, separated by an underscore) and submit it together with the submission ZIP.

**The submission deadline (date and time), submission form and upload link, and contact channel will be announced on the day of the event.**

### Troubleshooting

- **If installation fails:** Check the error message in Setup A and your internet connection, then run the cell again.
- **After restarting a session or kernel:** Variables and function definitions are cleared even if earlier outputs remain visible. Rerun the required cells in order, beginning with Setup A.
- **If the automatic Colab download does not start:** Check the displayed file path and download the ZIP from Colab's file panel on the left.
- **If a Jupyter download link comes from an earlier saved output:** Run all cells again and use the new link displayed by the final cell.

If a problem persists, send the error message and identify the affected cell through the contact channel announced by the organizers. See the notebook for the requirements of each exercise and the [scoring rubric](https://github.com/equivoque-jk/qff-2026-grader/blob/main/docs/SCORING.md) for the detailed point allocation.
