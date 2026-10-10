# Swing Tracer

골프 스윙 영상을 올리면 손 궤적을 트레이스하고, 클럽·체형별 기준으로 자세와 템포를 진단해 교정법을 알려주는 웹앱입니다. 골프존·트랙맨 같은 시뮬레이터 수치(볼 스피드, 발사각, 스핀 등)를 넣으면 구질과 개선 방향도 분석합니다.

- 영상은 브라우저 안에서만 분석되며 서버로 전송되지 않습니다.
- 포즈 추정: Google MediaPipe Pose Landmarker (Apache 2.0)

## 배포 (GitHub Pages)
1. 이 폴더의 파일을 저장소 루트에 올립니다.
2. Settings → Pages → Source: `Deploy from a branch`, Branch: `main` / `(root)` → Save.
3. 1–2분 뒤 `https://<아이디>.github.io/<저장소이름>/` 에서 열립니다.

## 로컬 실행
```
python3 -m http.server 8000
```
브라우저에서 http://localhost:8000 을 엽니다. (파일을 더블클릭해서 열면 모델 로딩이 막힙니다.)
