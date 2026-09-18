# Team Project Memo

팀 프로젝트에 들어가기 전 Git 브랜치와 화면 단위 협업 방식을 연습하기 위해 만든 Flutter 메모 앱 작업 저장소입니다. 메모 모델과 작성·편집 화면 일부가 준비되어 있지만, 현재 실행 진입점에는 아직 연결되지 않은 진행 중 프로젝트입니다.

## 현재 구현된 작업

- 메모 데이터 모델 초안
- 제목 입력 및 본문 편집 위젯
- 메모 추가·편집 화면 구조
- 화면별 State·ViewModel 파일 배치
- 기능 단위 폴더 구조 실험

## 기술 스택

- Flutter / Dart
- Material Design
- Git 브랜치 기반 협업 연습

## 구조

```text
lib/
├── data/model/          # 메모 모델
├── feature/note_edit/   # 편집 화면, 상태, ViewModel, 위젯
├── view/note/note_add/  # 추가 화면, 상태, ViewModel
└── main.dart            # 현재는 Flutter 기본 카운터 화면
```

## 실행 방법

이 저장소의 작업 브랜치는 `develop`입니다.

```bash
git clone -b develop https://github.com/YunFlutter/Team_project_memo.git
cd Team_project_memo
flutter pub get
flutter run
```

## 프로젝트 상태

현재 `main.dart`는 Flutter 기본 카운터 앱을 실행합니다. 메모 화면 파일은 존재하지만 앱의 라우팅 및 상태 흐름에 연결되지 않았고, 일부 ViewModel은 구현 전 상태입니다. 따라서 이 저장소는 완성된 메모 앱이 아닌 협업 전 연습 기록으로 분류합니다.

## 다음 단계

- 기본 카운터 화면을 메모 목록 화면으로 교체
- 추가·편집 화면 라우팅 연결
- ViewModel과 상태 변경 로직 구현
- 로컬 저장소 또는 데이터베이스 연동
- 입력 검증, 테스트, 빈 상태·오류 상태 UI 추가
