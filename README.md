# sprknd.github.io

SUPERKIND 소개 페이지(https://sprknd.github.io). 빌드 없는 한 장짜리 정적 페이지입니다.

- `index.html`: 페이지 전체(스타일과 스크립트 포함). 마스코트 프레임은 supacctv의 `tools/mascot/mascot.py`에서 뽑았습니다.
- `app-ads.txt`: AdMob 게시자 줄. BOINY와 BEONY가 같이 씁니다. 스토어의 개발자 웹사이트가 이 사이트여야 AdMob이 읽습니다.
- main에 push하면 `.github/workflows/pages-deploy.yml`이 GitHub Pages로 올립니다. 올릴 파일을 늘리면 그 워크플로의 `cp` 목록에도 넣습니다.

예전 Jekyll(Chirpy) 블로그는 커밋 3bb9234에 남아 있습니다.
