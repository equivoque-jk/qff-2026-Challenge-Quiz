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

**The notebook you choose contains all exercise descriptions, figures, experiment code, and the grader installation cell.** To download it, open the notebook file page and select **Download raw file**. The same file works in Colab, VS Code, and Jupyter.

## Getting started

1. If you open the notebook in Colab, **save your own copy**. In VS Code or Jupyter, open the downloaded `.ipynb` file.
2. Use a **CPU runtime** in Colab or a **Python 3.10–3.13 kernel** in VS Code or Jupyter. **Python 3.12** is recommended for local use.
3. **Run only Setup A first.** It installs [Grader 2.0.6](https://github.com/equivoque-jk/qff-2026-grader/releases/tag/v2.0.6) and the tools required for the experiments. An internet connection is required for the initial installation.
4. If prompted to restart, select **Runtime → Restart session** in Colab, or **restart the kernel** in VS Code or Jupyter. Then run Setup A again.
5. Once setup is complete, run Setup B, C, and D, followed by the provided tools and exercise cells in order.

## Exercise structure

| Part | Content | Points |
|---|---|---:|
| 1. Measurement and Entanglement | Distinguish states through measurement bases and prepare Bell and GHZ resources | 30 |
| 2. Quantum Teleportation | Diagnose, repair, and verify a faulty teleportation circuit | 40 |
| 3. GHZ–Mermin Game | Compare the winning probabilities of classical and quantum strategies | 30 |
| Optional 2-5 | Transfer the full state of two qubits | 12 additional |
| Optional 3-5 | Analyze game performance with phase errors in the shared resource | 8 additional |

The **14 core exercises are worth 100 points**, and the **two optional exercises offer 20 additional points**. You may complete either or both optional exercises. Leaving them unanswered does not affect your core score.

## Completing the exercises

- Write your code **between `TODO BEGIN` and `TODO END`** in each answer function. Remove the `raise NotImplementedError(...)` statement in that region and replace it with your implementation.
- Preserve function signatures, provided initialization code, final `return` statements, and the execution and grading cells. There are 23 answer functions, including the optional exercises.
- Read each exercise's **return format and grading criteria**. Numerical answers must return the exact values requested in the exercise; do not copy estimates from sampling experiments.
- Use the Experiment Notes to record your calculations and interpret the results. The notes and the final Network Commissioning Report are not graded.

**The failure messages from the provided faulty circuits in 2-1 and optional 2-5 are intentional.** Use them to identify the defects, then verify that your repaired circuits pass the checks.

## Grading and submission

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

## Troubleshooting

- **If installation fails:** Check the error message in Setup A and your internet connection, then run the cell again.
- **After restarting a session or kernel:** Variables and function definitions are cleared even if earlier outputs remain visible. Rerun the required cells in order, beginning with Setup A.
- **If the automatic Colab download does not start:** Check the displayed file path and download the ZIP from Colab's file panel on the left.
- **If a Jupyter download link comes from an earlier saved output:** Run all cells again and use the new link displayed by the final cell.

If a problem persists, send the error message and identify the affected cell through the contact channel announced by the organizers. See the notebook for the requirements of each exercise and the [scoring rubric](https://github.com/equivoque-jk/qff-2026-grader/blob/main/docs/SCORING.md) for the detailed point allocation.
