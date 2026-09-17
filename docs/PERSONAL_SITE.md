# 블로그 관리

- 기본 정보와 블로그 이름: `_config.yml`
- 자기소개: `_pages/about.md`
- 연락처: `_data/socials.yml`
- 이력서 및 논문 원본 데이터: `_data/cv.yml`
- 논문 페이지: `_pages/publications.md` (이력서의 Publications 데이터를 사용)
- 강의 경력: `_pages/teaching.md`
- 블로그 글: `_posts/YYYY-MM-DD-title.md`

프로필 사진은 아직 설정하지 않았습니다. 사진을 `assets/img/`에 추가한 뒤 `_pages/about.md`의 `profile: false`를 사진 설정으로 바꾸면 됩니다.

기존 예제 글과 페이지는 `_template_examples/`에 보관되어 있으며 사이트에 게시되지 않습니다. 파일을 복사해 새 글의 서식 참고용으로 쓸 수 있습니다.

CV에 기재되지 않은 논문 연도, 학위 지도교수, 프로필 사진 및 Google Scholar ID는 추가하지 않았습니다. CV에서 `et al.`로 생략한 저자 목록도 그대로 유지했습니다. 예제 PDF 다운로드 링크는 제거했습니다.

사이트는 저장소 루트 주소를 사용합니다. 로컬 실행 시 `_config.yml`의 빈 `baseurl`을 유지하세요.

## 로컬 미리보기

현재 컴퓨터에서는 `bin/preview.command`를 더블클릭하거나 아래 명령으로 실행할 수 있습니다.

```bash
cd ~/Desktop/statduck.github.io
./bin/preview.command
```

브라우저에서 `http://127.0.0.1:4000`을 여세요. 파일을 저장한 뒤 페이지를 새로고침하면 수정 결과를 확인할 수 있습니다. `_config.yml`을 수정하면 서버를 다시 실행하세요. 서버 종료는 실행한 터미널에서 Control-C입니다.

이 실행 파일은 `vendor/`에 설치된 Ruby와 패키지를 사용합니다. `vendor/`는 Git에 포함되지 않으므로 다른 컴퓨터에서는 환경을 다시 설치해야 합니다. 미리보기에서는 이미지 크기 변환을 끄며, 실제 배포 설정은 유지됩니다.
