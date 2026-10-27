# QFF 2026 Hackathon

QFF 2026 Q-LINK 참가자용 문제지입니다. **문제지 ver3 · 채점 패키지 2.0.2**를 사용합니다.

**`QFF_Challenge_Colab.ipynb` 하나만 받으면 됩니다.** 문제 설명, 이미지, 실험 코드와 채점 패키지 설치 셀이 모두 들어 있습니다. 준비 A를 실행하면 GitHub Release의 지정된 grader와 필요한 실험 도구를 자동 설치합니다.

- [문제지 파일·다운로드](https://github.com/equivoque-jk/qff-2026-Hackathon/blob/main/QFF_Challenge_Colab.ipynb)
- [Google Colab에서 바로 열기](https://colab.research.google.com/github/equivoque-jk/qff-2026-Hackathon/blob/main/QFF_Challenge_Colab.ipynb)
- [GitHub에서 문제지 보기](QFF_Challenge_Colab.ipynb)

문제지 파일 화면에서 **Download raw file** 버튼을 누르면 `.ipynb` 하나를 저장할 수 있습니다. Colab을 사용한다면 위의 바로 열기 링크로 시작해도 됩니다.

## 실행 환경

| 환경 | 시작 방법 |
|---|---|
| Google Colab | 위의 바로 열기 링크를 사용하거나, 내려받은 `.ipynb`를 Colab에 업로드합니다. CPU 런타임으로 실행할 수 있습니다. 풀이를 보관할 수 있도록 자신의 사본으로 저장하세요. |
| VS Code | Python과 Jupyter 확장이 준비된 환경에서 `.ipynb`를 열고 Python 커널을 선택합니다. |
| Jupyter Notebook / JupyterLab | 내려받은 `.ipynb`를 열고 Python 커널을 선택합니다. |

**Python 3.10–3.13을 지원하며 로컬 환경은 3.12를 권장합니다.** VS Code·Jupyter에서는 노트북을 실행할 Python 커널이 먼저 준비되어 있어야 합니다. 준비 A는 현재 커널의 Python에 패키지를 설치하므로, 사용할 환경을 선택한 뒤 실행하세요. 최초 설치에는 GitHub와 Python 패키지 배포 사이트에 접속할 수 있는 인터넷 연결이 필요합니다.

## 풀이 순서

1. **준비 A 셀만 먼저 실행**합니다. grader와 실험 도구가 자동 설치되며 진행 로그가 표시됩니다.
2. 재시작 안내가 나오면 Colab에서는 **런타임 → 세션 다시 시작**, VS Code·Jupyter에서는 **커널 재시작**을 선택한 뒤 준비 A를 다시 실행합니다. 이미 필요한 버전이 설치되어 있으면 설치를 건너뜁니다.
3. 준비 B·C·D와 해당 문제에 필요한 제공 도구·문제 셀을 순서대로 실행합니다.
4. 문제지의 23개 답안 함수에서 `TODO BEGIN`과 `TODO END` 사이를 작성합니다. 그 안의 `raise NotImplementedError(...)`를 자신의 구현으로 교체하세요. 미작성 선택 문항은 TODO를 그대로 둘 수 있습니다.
5. 전체 답안을 채점하고 제출 파일을 만들 때 **모두 실행 / Run All**을 선택합니다. 마지막 셀이 채점 결과와 답안 제출용 ZIP을 생성합니다.
6. **답안 제출 ZIP과 작성한 `.ipynb`를 공지된 제출처에 함께 제출**합니다. 노트북은 제출 ZIP에 자동 포함되지 않으므로 별도로 저장하세요.

Colab에서는 제출 ZIP 다운로드가 시작됩니다. VS Code·Jupyter에서는 출력에 표시된 다운로드 링크 또는 저장 경로에서 파일을 가져올 수 있습니다. 로컬 채점과 파일 생성은 공식 제출 접수가 아니므로, 행사에서 안내한 제출 절차를 완료해야 합니다.

## 채점 패키지

채점기는 별도 저장소 [qff-2026-grader](https://github.com/equivoque-jk/qff-2026-grader)에서 관리합니다. 이 문제지의 준비 A는 [Release v2.0.2](https://github.com/equivoque-jk/qff-2026-grader/releases/tag/v2.0.2)의 wheel URL과 SHA-256을 고정하여 설치합니다. 이미지 파일이나 wheel, 통합 배포 ZIP을 따로 받을 필요는 없습니다.

기본 100점과 선택 심화 추가 20점으로 총점 상한은 120점입니다. 정확한 반환 형식과 채점 조건은 문제지의 각 문항을 따르세요. 배점과 반환 계약의 상세 설명은 [grader 저장소](https://github.com/equivoque-jk/qff-2026-grader)에 있습니다.

패키지 2.0.2에서는 손상된 답안 ZIP 하나가 운영진의 전체 일괄 채점을 중단시키던 문제를 수정했습니다. 이번 문제지 변경은 설치 버전·Release 링크·해시에 한정되며, 기존 ver3의 문제 내용·답안 함수·제공 코드·배점은 동일합니다.

환경 설정에 관한 자세한 설명은 [VS Code의 Jupyter 안내](https://code.visualstudio.com/docs/datascience/jupyter-notebooks), [JupyterLab의 노트북 안내](https://jupyterlab.readthedocs.io/en/stable/user/notebook.html)를 참고하세요.
