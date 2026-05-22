# 작업 흐름 정리

## 논문 하나 리뷰할 때 전체 순서

```
1. 논문 읽기
      ↓
2. 티스토리에 리뷰 글 작성 (이론 정리, 이미지 첨부)
      ↓
3. Jupyter Notebook에서 코드 구현
      ↓
4. GitHub에 올리기
      ↓
5. README 목록 업데이트
```

---

## 각 단계 상세

### ① 티스토리 — 이론 정리 (지금처럼 그대로)
- 논문 내용, 수식 설명, 그림 등 글로 정리
- 변경 없음

### ② Jupyter Notebook — 코드 구현
- 경로: `C:\Users\dogun\Downloads\Desktop\Desktop\Desktop\Desktop\김건도\Github\Paper-Review`
- 해당 폴더(`RNN`, `Vision`, `NLP`, `Generative`)에 `.ipynb` 파일 생성
- 노트북 상단에 티스토리 링크 달아두면 연결됨

```markdown
# [논문리뷰] ViT
티스토리 리뷰: https://dogun5578.tistory.com/...
```

### ③ GitHub 업로드 — 터미널에서 3줄
```powershell
cd "C:\Users\dogun\Downloads\Desktop\Desktop\Desktop\Desktop\김건도\Github\Paper-Review"
git add .
git commit -m "add: ViT 리뷰"
git push origin main
```

### ④ README 업데이트 — 표에 한 줄 추가
```markdown
| Vision Transformer (ViT) | 2020 | [📓 보기](Vision/ViT.ipynb) |
```

---

## 역할 분리 요약

| 플랫폼 | 역할 |
|--------|------|
| **티스토리** | 이론 설명, 수식, 그림 → 읽기 편한 글 |
| **GitHub Notebook** | 코드 구현, 실험 결과 → 직접 돌려볼 수 있는 코드 |
| **GitHub README** | 전체 목록 정리 → 포트폴리오 대문 |

---

## 폴더 구조

```
Paper-Review/
├── README.md        ← 전체 목록 (대문)
├── WORKFLOW.md      ← 이 파일
├── RNN/
│   └── LSTM.ipynb
├── Vision/
│   └── ViT.ipynb
├── NLP/
│   └── Attention.ipynb
└── Generative/
    └── DDPM.ipynb
```
