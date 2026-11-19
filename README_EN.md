![Qiskit Fall Fest 2026 at Korea University](assets/readme/qiskit-fall-fest-2026-korea-university.jpg)

# QFF 2026 — Q-LINK

**Qiskit Fall Fest · QUICK · Korea University | Participant Edition**

[한국어 안내](README.md#한국어-안내) · **English guide** · [Bilingual README](README.md#english-guide)

Join a quantum network experiment connecting the laboratories of Alice, Bob, and Charlie. Inspect measurement equipment and entanglement resources, transfer a quantum state by teleportation, and evaluate how the three laboratories cooperate in the GHZ–Mermin game.

**Run this hackathon notebook only in Google Colab.** Each participant works in their own Drive copy and submits their own completed notebook and submission ZIP.

## Choose your language

| Language | Google Colab | Notebook file | Guide |
|---|---|---|---|
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab_EN.ipynb) | [QFF_Challenge_Colab_EN.ipynb](QFF_Challenge_Colab_EN.ipynb) | This README |
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Challenge-Quiz/blob/main/QFF_Challenge_Colab.ipynb) | [QFF_Challenge_Colab.ipynb](QFF_Challenge_Colab.ipynb) | [한국어 안내](README.md#한국어-안내) |

Both editions have **the same exercises, structure, point allocation, and grading criteria**. Each notebook automatically selects its language for grading feedback and submission instructions; you do not need to edit any language settings.

The selected notebook contains the exercise descriptions, experiment code, and grader installation cell. Figures load automatically from this repository's [`assets`](assets/) folder, so **an internet connection is required to display them**. You do not need to upload image files or clone the repository. If you need a downloaded notebook, open its file page and select **Download raw file**, then open that `.ipynb` in Colab.

The image URLs become accessible without separate repository authorization when this repository is made public for the event. Access remains restricted while the repository is private before distribution.

## Getting started

**Save and rename your own copy before running the setup cells or starting the exercises.**

1. **Open the notebook from GitHub.** Sign in to [Google Colab](https://colab.research.google.com/) with your own Google account. Choose **File → Open notebook**, select the **GitHub** tab, and search for the repository URL below:

   [https://github.com/equivoque-jk/qff-2026-Challenge-Quiz](https://github.com/equivoque-jk/qff-2026-Challenge-Quiz)

   Select **`QFF_Challenge_Colab_EN.ipynb`** for the English edition. You can also open it directly using the **Open in Colab** link in the table above.

2. Choose **File → Save a copy in Drive**. Continue in the newly opened **copy in your own Drive**. Your edits and saved work belong to this copy and do not update the distribution repository.<br>
   In your copy, open **Edit → Notebook settings → AI Assistance** and check that **Hide generative AI features** is selected.<br>
   If you are using an earlier copy and the box is unchecked, select it and save your copy.

3. **Click the copied notebook's title at the top and rename it to `학번_이름.ipynb`** (your student ID and name, separated by an underscore).

4. Use a **CPU runtime** and **run only Setup A first**. It installs the **bundled Grader 2.2.0** and the required experiment tools. An internet connection is required for the initial installation. Packages are not reinstalled if the required versions are already available.

5. **Only if prompted to restart**, select **Runtime → Restart session**, then run Setup A again.

6. Once the setup completion message appears, run **Setup B, C, and D**, then work through each part's provided tools and exercise cells in order.

7. After completing your answers, select **Runtime → Run all** to generate the grading results and submission ZIP in the final cell. Save both required files as explained in **Grading and submission** below.

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
- Preserve function signatures, provided initialization code, final `return` statements, and all provided helper, execution, and grading cells. There are **25 answer functions**, including the optional exercises.
- Leave the TODO regions unchanged for optional exercises you choose not to complete.
- Read each exercise's **return format and grading criteria**. Numerical answers must return the exact values requested in the exercise; do not copy estimates from sampling experiments.
- Use the Experiment Notes to record your calculations and interpret the results. The notes and the final Network Commissioning Report are not graded.

**The failure messages from the provided faulty circuits in 2-1 and optional 2-5 are intentional.** Use them as evidence to analyze the defects and complete the answers requested by each exercise.

## Grading and submission

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

## Troubleshooting

- **If a figure does not load:** Check your internet connection and whether your network allows access to `raw.githubusercontent.com`, then refresh the page. Displaying figures does not require a runtime connection or running the setup cells. Image access is restricted before the repository's event-day public release.
- **If installation fails:** Check the error message in Setup A and your internet connection, then run the cell again.
- **After restarting the session:** Variables and function definitions are cleared even if earlier outputs remain visible. Rerun the required cells in order, beginning with Setup A.
- **If the automatic ZIP download does not start:** Check the displayed save path and download the ZIP from Colab's Files panel on the left.

If a problem persists, show the organizers the error message and identify the affected cell. The [English notebook](QFF_Challenge_Colab_EN.ipynb) gives the requirements, point allocation, and grading criteria for each exercise.
