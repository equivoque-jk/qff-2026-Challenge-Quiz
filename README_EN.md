# QFF 2026 — Q-LINK

**Qiskit Fall Fest · QUICK · Korea University | Participant Edition**

[한국어 안내](README.md#한국어-안내) · **English guide** · [Bilingual README](README.md#english-guide)

Join a quantum network experiment connecting the laboratories of Alice, Bob, and Charlie. Inspect measurement equipment and entanglement resources, transfer a quantum state by teleportation, and evaluate how the three laboratories cooperate in the GHZ–Mermin game.

## Choose your language

| Language | Google Colab | Notebook file | Guide |
|---|---|---|---|
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | This README |
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [한국어 안내](README.md#한국어-안내) |

Both editions have **the same exercises, structure, point allocation, and grading criteria**. Each notebook automatically selects its language for grading feedback and submission instructions; you do not need to edit any language settings.

**The notebook you choose contains all exercise descriptions, experiment code, and the grader installation cell.** Figures load automatically from this repository's [`assets`](assets/) folder, so **an internet connection is also required to display them.** You do not need to upload image files or clone the repository. To download the notebook, open its file page and select **Download raw file**. Participants complete the exercises in **Google Colab**.

The image URLs become accessible without separate authorization when this repository is made public for the event. Access remains restricted while the repository is private before distribution.

## Getting started

1. Open the notebook using the Colab link above and **save a copy to your own Drive**.
2. Use a **CPU runtime** in Colab.
3. **Run only Setup A first.** It installs the bundled Grader 2.2.0 and the tools required for the experiments. An internet connection is required for the initial installation.
4. **Only if prompted to restart**, select **Runtime → Restart session**, then run Setup A again.
5. Once setup is complete, run Setup B, C, and D, followed by the provided tools and exercise cells in order.

## Exercise structure

| Part | Content | Points |
|---|---|---:|
| 1. Measurement and Entanglement | Distinguish states through measurement bases and prepare Bell and GHZ resources | 30 |
| 2. Quantum Teleportation | Diagnose, repair, and verify a faulty teleportation circuit | 40 |
| 3. GHZ–Mermin Game | Compare the winning probabilities of classical and quantum strategies | 30 |
| Optional 2-5 | Transfer the full state of two qubits | 12 additional |
| Optional 3-5 | Analyze game performance with phase errors in the shared resource | 8 additional |

Exercise 1-5 awards **5 points for circuit preparation and 2 points for the correlation table**, graded independently. Exercise 2-2 also grades its parts independently: **4 points for the states before correction and 14 points for repairing the teleportation circuit**.

The **14 core exercises are worth 100 points**, and the **two optional exercises offer 20 additional points**. You may complete either or both optional exercises. Leaving them unanswered does not affect your core score.

## Completing the exercises

- Write your code **between `TODO BEGIN` and `TODO END`** in each answer function. Remove the `raise NotImplementedError(...)` statement in that region and replace it with your implementation.
- Preserve function signatures, provided initialization code, final `return` statements, and the execution and grading cells. There are 25 answer functions, including the optional exercises.
- Read each exercise's **return format and grading criteria**. Numerical answers must return the exact values requested in the exercise; do not copy estimates from sampling experiments.
- Use the Experiment Notes to record your calculations and interpret the results. The notes and the final Network Commissioning Report are not graded.

**The failure messages from the provided faulty circuits in 2-1 and optional 2-5 are intentional.** Use them to identify the defects, then verify that your repaired circuits pass the checks.

## Grading and submission

1. Save your answers, then select **Runtime → Run all**. Leave the TODOs unchanged for optional exercises you have not attempted.
2. In the final cell, check your **core and additional scores, incomplete items, and errors**. Experiment outputs and checks of answer-function return values serve different purposes, so always inspect the final grading result.
3. Save the **submission ZIP** as described below, and **save the completed notebook separately as an `.ipynb` file**. The notebook is not included in the ZIP. In Colab, download both files before ending the runtime.
4. **Submit both the ZIP and your completed `.ipynb` to the destination announced by the event organizers.**

| File to save | How to save it in Colab |
|---|---|
| Submission ZIP | The final cell requests an automatic browser download. If it does not start, check the printed path and download that ZIP from the Files panel on the left. |
| Completed notebook | **File → Download → Download .ipynb** |

After editing your answers and running all cells again, the results are saved under a new run ID. **Check that the run ID in the final grading result matches the submission ZIP.** Running the grading cell and saving files does not by itself submit your work.

**Submissions are individual.** Name your completed notebook **`학번_이름.ipynb`** (student ID and name, separated by an underscore) and submit it together with the submission ZIP.

**The submission deadline (date and time), submission form and upload link, and contact channel will be announced on the day of the event.**

## Troubleshooting

- **If a figure does not load:** Check your internet connection and whether your network allows access to `raw.githubusercontent.com`, then refresh the page. Displaying figures does not require a runtime connection or running the setup cells.
- **If installation fails:** Check the error message in Setup A and your internet connection, then run the cell again.
- **After restarting the session:** Variables and function definitions are cleared even if earlier outputs remain visible. Rerun the required cells in order, beginning with Setup A.
- **If the automatic Colab download does not start:** Check the displayed file path and download the ZIP from Colab's file panel on the left.

If a problem persists, send the error message and identify the affected cell through the contact channel announced by the organizers. See the notebook for the requirements of each exercise and the [scoring rubric](https://github.com/equivoque-jk/qff-2026-grader/blob/main/docs/SCORING.md) for the detailed point allocation.
