![Qiskit Fall Fest 2026 at Korea University](assets/readme/qiskit-fall-fest-2026-korea-university.jpg)

# QFF 2026 — Q-LINK

[한국어 안내](#한국어-안내) · [English guide](#english-guide)

## 한국어 안내

**Qiskit Fall Fest · QUICK · 고려대학교 | 참가자용**

Alice, Bob, Charlie의 세 실험실을 연결하는 양자 네트워크 실험에 참여하세요. 측정과 얽힘 자원을 점검하고, 양자 텔레포테이션으로 상태를 전송한 뒤, GHZ–Mermin 게임에서 세 실험실의 협력 성능을 확인합니다.

**해커톤은 Google Colab에서만 진행합니다.** 참가자는 자신의 Drive 사본에서 풀이하고, 각자의 풀이 노트북과 제출 ZIP을 제출합니다.

### 언어 선택 · Choose your language

| 언어 / Language | Google Colab | 노트북 파일 / Notebook | 사용 안내 / Guide |
|---|---|---|---|
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](QFF_Challenge_Colab.ipynb) | [한국어 안내](#한국어-안내) |
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](QFF_Challenge_Colab_EN.ipynb) | [English guide](#english-guide) |

**English participants:** Open the English notebook above and follow the [English guide](#english-guide). The notebook selects English grading feedback automatically.

두 언어의 **문제·구성·배점·채점 기준은 동일**합니다. 각 노트북은 해당 언어의 채점 피드백과 제출 안내를 자동으로 표시하므로 언어 설정 코드를 수정할 필요가 없습니다.

문제 설명, 실험 코드와 채점 도구 설치 셀은 **선택한 노트북 하나에 들어 있습니다.** 그림은 이 저장소의 [`assets`](assets/) 폴더에서 자동으로 불러오므로 **이미지 표시에도 인터넷 연결이 필요합니다.** 별도의 이미지 파일 업로드나 저장소 복제는 필요하지 않습니다. 내려받으려면 노트북 파일 화면의 **Download raw file** 버튼을 누르세요. 참가자 실습은 **Google Colab에서만 진행합니다.**

그림 주소는 행사 배포를 위해 저장소를 공개한 뒤 별도 인증 없이 사용할 수 있습니다. 배포 전 비공개 상태에서는 이미지 주소에 대한 접근이 제한됩니다.

### 시작하기

**Google Colab에서만 실행합니다.** Colab의 **CPU 런타임**을 사용하세요.

**아래 순서로 개인 풀이 노트북을 준비한 뒤 실험을 시작하세요.**

1. **GitHub 저장소에서 문제지를 불러오세요.**<br>
   자신의 Google 계정으로 [Colab](https://colab.research.google.com/)에 로그인한 뒤, **파일 → 노트북 열기(Open notebook) → GitHub**에서 아래 저장소 주소를 검색하세요.<br>
   [https://github.com/equivoque-jk/qff-2026-Challenge-Quiz](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz)<br>
   목록에서 한국어판 <strong><code>QFF_Challenge_Colab.ipynb</code></strong>를 선택하세요.<br>
   위의 **Colab에서 시작하기** 링크로 바로 열어도 됩니다.

2. **파일 → Drive에 사본 저장**을 선택하세요.<br>
   이후 풀이와 실행은 새로 열린 **자신의 Drive 사본**에서 진행합니다.<br>

3. **화면 상단의 사본 이름을 눌러 `학번_이름.ipynb`로 바꾸세요.**<br>
   **사본 저장과 이름 변경을 마친 뒤** 아래 준비 셀을 실행하고 풀이를 시작하세요.

4. **먼저 준비 A 셀만 실행하세요.**<br>
   **문제지에 포함된 채점기 2.2.0**과 실험 도구를 설치합니다.<br>
   필요한 버전이 이미 설치되어 있으면 재설치하지 않습니다.<br>
   준비 A에서 채점기 데이터를 불러오라는 안내가 나오면 바로 위의 접힌 **채점기 패키지 데이터** 셀을 실행한 뒤 준비 A를 다시 실행하세요.

5. **재시작 안내가 나온 경우에만** **런타임 → 세션 다시 시작**을 선택하고 준비 A를 다시 실행하세요.

6. 준비 완료 메시지가 나오면 **준비 B·C·D**를 실행하고, 각 파트의 제공 도구와 문제 셀을 위에서부터 진행하세요.

7. 풀이를 마친 뒤 **런타임 → 모두 실행**을 선택하면 마지막 셀에서 채점 결과와 제출 ZIP을 생성합니다.<br><br>
   제출은 개인 단위로 진행합니다.<br>
   **풀이 노트북을 `학번_이름.ipynb`로 저장**하여 ZIP과 함께 제출하세요.

### 문제 구성

| 구분 | 내용 | 배점 |
|---|---|---:|
| 1. 측정과 얽힘 | 측정 기저에 따른 상태 구별과 Bell·GHZ 자원 준비 | 30점 |
| 2. 양자 텔레포테이션 | 고장 회로 진단, 전송 회로 복구와 검증 | 40점 |
| 3. GHZ–Mermin 게임 | 고전 전략과 양자 전략의 승률 비교 | 30점 |
| 선택 2-5 | 두 큐비트의 전체 상태 전송 | 추가 12점 |
| 선택 3-5 | 위상 오류가 있는 자원의 게임 성능 분석 | 추가 8점 |

1-5는 **회로 준비 5점 + 상관값 표 2점**으로 구성하며 두 부분을 독립적으로 채점합니다. 2-2도 **보정 전 상태 계산 4점 + 전송 회로 복구 14점**을 독립적으로 채점합니다.

기본 **14문항은 100점**, 선택 **2문항은 추가 20점**입니다. 선택 문항은 원하는 문제만 풀 수 있으며, 풀지 않아도 기본 문항 점수에는 영향을 주지 않습니다.

### 풀이 방법

- 답안 함수의 **`TODO BEGIN`과 `TODO END` 사이**에 코드를 작성하세요. 해당 영역의 `raise NotImplementedError(...)`를 지우고 자신의 구현으로 교체하세요.
- 함수 선언, 제공된 초기화 코드, 마지막 `return`, 제공 도구·실행·채점 셀은 그대로 두세요. 답안 함수는 선택 문항을 포함해 **총 25개**입니다.
- 풀지 않는 선택 문항의 TODO는 그대로 두세요.
- 각 문항의 **반환 형식과 채점 사항**을 확인하세요. 수치 답안에는 표본 실험의 추정치를 복사하지 말고, 문제에서 요구하는 정확한 값을 계산해 반환하세요.
- 실험 메모에는 계산 과정과 결과를 해석한 내용을 적으세요. 실험 메모와 마지막 개통 보고서는 채점 대상이 아닙니다.

**2-1과 선택 2-5에서 제공된 고장 회로의 실패 메시지는 의도된 결과입니다.** 메시지를 단서로 문항 지시에 따라 결함을 분석하고 답안을 작성하세요.

### 채점 및 제출

1. 답안을 저장한 뒤 준비 A부터 **런타임 → 모두 실행**을 진행하세요. 작성하지 않은 선택 문항의 TODO는 그대로 두세요.

2. 마지막 셀에서 **기본·추가 점수와 미완성·오류 항목**을 확인하세요. 문제별 실험 출력과 답안 함수의 반환값 검사는 다르므로 마지막 채점 결과도 확인해야 합니다.

3. **제출 ZIP**과 **`학번_이름.ipynb`로 작성한 풀이 노트북**을 각각 다운로드하세요. 노트북은 **제출 ZIP에 포함되지 않습니다.** Colab 런타임을 종료하기 전에 두 파일을 내려받으세요.

4. **두 파일을 행사에서 안내한 제출처에 함께 제출**하세요. 제출은 개인 단위로 진행합니다.

| 제출할 파일 | Colab에서 저장하는 방법 |
|---|---|
| `QFF_<실행 ID>.zip` | 마지막 셀이 브라우저에 자동 다운로드를 요청합니다. 시작되지 않으면 출력된 경로를 확인하고 왼쪽 파일 패널에서 해당 ZIP을 다운로드하세요. |
| `학번_이름.ipynb` | 노트북 이름을 확인한 뒤 **파일 → 다운로드 → .ipynb 다운로드**를 선택하세요. |

답안을 수정하고 다시 모두 실행하면 **새 실행 ID**로 결과가 저장됩니다. 마지막 출력의 **`실행 기록:` 뒤 식별자**와 ZIP 파일명 **`QFF_<실행 ID>.zip`의 식별자**가 같은지 확인하고, 해당 실행이 끝난 뒤 풀이 노트북도 다시 다운로드하세요. 이전 실행의 파일은 덮어쓰지 않습니다.

**채점 셀 실행과 파일 생성만으로 제출이 접수되지는 않습니다.** 공지된 제출처에 ZIP과 노트북을 직접 제출해야 합니다.

**마감 날짜·시각과 제출 폼·업로드 링크는 행사 당일 공지에 따릅니다.**

### 실행 중 문제가 생겼다면

- **그림이 표시되지 않을 때:** 인터넷 연결과 `raw.githubusercontent.com` 접근 가능 여부를 확인한 뒤 페이지를 새로고침하세요. 그림 표시에는 런타임 연결이나 준비 셀 실행이 필요하지 않습니다. 행사 당일 저장소 공개 전에는 이미지 접근이 제한됩니다.
- **설치가 실패할 때:** 준비 A의 오류 메시지와 인터넷 연결을 확인한 뒤 다시 실행하세요.
- **세션을 다시 시작했을 때:** 화면에 예전 출력이 남아 있어도 변수와 함수 정의는 사라집니다. 준비 A부터 필요한 셀을 순서대로 다시 실행하세요.
- **Colab 자동 다운로드가 시작되지 않을 때:** 마지막 셀에 표시된 저장 경로를 확인하고, Colab 왼쪽 파일 패널에서 해당 ZIP을 다운로드하세요.

해결되지 않는 문제가 생기면 오류 메시지와 해당 셀을 운영진에게 보여 주세요. 자세한 문항 조건·배점·채점 기준은 [한국어 노트북](QFF_Challenge_Colab.ipynb)의 각 문항과 「채점 사항」을 확인하세요.

---

## English Guide

**Qiskit Fall Fest · QUICK · Korea University | Participant Edition**

Join a quantum network experiment connecting the laboratories of Alice, Bob, and Charlie. Inspect measurement equipment and entanglement resources, transfer a quantum state by teleportation, and evaluate how the three laboratories cooperate in the GHZ–Mermin game.

**Run this hackathon notebook only in Google Colab.** Each participant works in their own Drive copy and submits their own completed notebook and submission ZIP.

### Choose your language

| Language | Google Colab | Notebook file | Guide |
|---|---|---|---|
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](QFF_Challenge_Colab_EN.ipynb) | This section |
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](QFF_Challenge_Colab.ipynb) | [한국어 안내](#한국어-안내) |

Both editions have **the same exercises, structure, point allocation, and grading criteria**. Each notebook automatically selects its language for grading feedback and submission instructions; you do not need to edit any language settings.

The selected notebook contains the exercise descriptions, experiment code, and grader installation cell. Figures load automatically from this repository's [`assets`](assets/) folder, so **an internet connection is required to display them**. You do not need to upload image files or clone the repository. If you need a downloaded notebook, open its file page and select **Download raw file**, then open that `.ipynb` in Colab.

The image URLs become accessible without separate repository authorization when this repository is made public for the event. Access remains restricted while the repository is private before distribution.

### Getting started

**Save and rename your own copy before running the setup cells or starting the exercises.**

1. **Open the notebook from GitHub.** Sign in to [Google Colab](https://colab.research.google.com/) with your own Google account. Choose **File → Open notebook**, select the **GitHub** tab, and search for the repository URL below:

   [https://github.com/equivoque-jk/qff-2026-Challenge-Quiz](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz)

   Select **`QFF_Challenge_Colab_EN.ipynb`** for the English edition. You can also open it directly using the **Open in Colab** link in the table above.

2. Choose **File → Save a copy in Drive**. Continue in the newly opened **copy in your own Drive**. Your edits and saved work belong to this copy and do not update the distribution repository.<br>
   In your copy, open **Edit → Notebook settings → AI Assistance** and check that **Hide generative AI features** is selected.<br>
   If you are using an earlier copy and the box is unchecked, select it and save your copy.

3. **Click the copied notebook's title at the top and rename it to `학번_이름.ipynb`** (your student ID and name, separated by an underscore).

4. Use a **CPU runtime** and **run only Setup A first**. It installs the **bundled Grader 2.2.0** and the required experiment tools. An internet connection is required for the initial installation. Packages are not reinstalled if the required versions are already available.
   If Setup A asks you to load the grader data, run the collapsed **Grader package data** cell directly above it, then run Setup A again.

5. **Only if prompted to restart**, select **Runtime → Restart session**, then run Setup A again.

6. Once the setup completion message appears, run **Setup B, C, and D**, then work through each part's provided tools and exercise cells in order.

7. After completing your answers, select **Runtime → Run all** to generate the grading results and submission ZIP in the final cell. Save both required files as explained in **Grading and submission** below.

### Exercise structure

| Part | Content | Points |
|---|---|---:|
| 1. Measurement and Entanglement | Distinguish states through measurement bases and prepare Bell and GHZ resources | 30 |
| 2. Quantum Teleportation | Diagnose, repair, and verify a faulty teleportation circuit | 40 |
| 3. GHZ–Mermin Game | Compare the winning probabilities of classical and quantum strategies | 30 |
| Optional 2-5 | Transfer the full state of two qubits | 12 additional |
| Optional 3-5 | Analyze game performance with phase errors in the shared resource | 8 additional |

Exercise 1-5 awards **5 points for circuit preparation and 2 points for the correlation table**, graded independently. Exercise 2-2 also grades its parts independently: **4 points for the states before correction and 14 points for repairing the teleportation circuit**.

The **14 core exercises are worth 100 points**, and the **two optional exercises offer 20 additional points**. You may complete either or both optional exercises. Leaving them unanswered does not affect your core score.

### Completing the exercises

- Write your code **between `TODO BEGIN` and `TODO END`** in each answer function. Remove the `raise NotImplementedError(...)` statement in that region and replace it with your implementation.
- Preserve function signatures, provided initialization code, final `return` statements, and all provided helper, execution, and grading cells. There are **25 answer functions**, including the optional exercises.
- Leave the TODO regions unchanged for optional exercises you choose not to complete.
- Read each exercise's **return format and grading criteria**. Numerical answers must return the exact values requested in the exercise; do not copy estimates from sampling experiments.
- Use the Experiment Notes to record your calculations and interpret the results. The notes and the final Network Commissioning Report are not graded.

**The failure messages from the provided faulty circuits in 2-1 and optional 2-5 are intentional.** Use them as evidence to analyze the defects and complete the answers requested by each exercise.

### Grading and submission

1. Save your answers, then select **Runtime → Run all** to rerun the notebook from Setup A. Leave the TODOs unchanged for optional exercises you have not attempted.

2. In the final cell, check your **core and additional scores, incomplete items, and errors**. Experiment outputs and checks of answer-function return values serve different purposes, so always inspect the final grading result.

3. Save the **submission ZIP** and **download your completed notebook separately as `학번_이름.ipynb`**. The notebook is **not included in the ZIP**. Download both files before ending the Colab runtime.

4. **Submit both files to the destination announced by the event organizers.** Submissions are individual.

| File to submit | How to save it in Colab |
|---|---|
| `QFF_<run ID>.zip` | The final cell requests an automatic browser download. If it does not start, check the printed path and download that ZIP from the Files panel on the left. |
| `학번_이름.ipynb` | Check the notebook title, then choose **File → Download → Download .ipynb**. |

After editing your answers and running all cells again, the results are saved under a **new run ID**. Check that the identifier after **`Run ID:`** in the final output matches the identifier in **`QFF_<run ID>.zip`**, and download your notebook again after that run. Files from earlier runs are not overwritten.

**Running the grading cell and generating files does not register a submission.** You must submit the ZIP and notebook through the destination announced at the event.

The **submission deadline (date and time), submission form, and upload link** will be announced on the day of the event.

### Troubleshooting

- **If a figure does not load:** Check your internet connection and whether your network allows access to `raw.githubusercontent.com`, then refresh the page. Displaying figures does not require a runtime connection or running the setup cells. Image access is restricted before the repository's event-day public release.
- **If installation fails:** Check the error message in Setup A and your internet connection, then run the cell again.
- **After restarting the session:** Variables and function definitions are cleared even if earlier outputs remain visible. Rerun the required cells in order, beginning with Setup A.
- **If the automatic ZIP download does not start:** Check the displayed save path and download the ZIP from Colab's Files panel on the left.

If a problem persists, show the organizers the error message and identify the affected cell. The [English notebook](QFF_Challenge_Colab_EN.ipynb) gives the requirements, point allocation, and grading criteria for each exercise.
