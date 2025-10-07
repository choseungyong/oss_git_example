# OSS Lecture Notes

> **오픈소스소프트웨어 실습 과제**
> Markdown 문법을 활용한 README.md 작성

---

## *Week 1-1* — **강의 개요 (강의계획서)**

> “Git/GitHub을 이용한 협업과 Haskell을 통한 함수형 프로그래밍 학습”
- [**강의계획서**](https://hakstd.jnu.ac.kr/Common/Syllabus/View200.aspx?YY=2025&SYLLABUS_KIND=C29020&EMPNO=48168&TERM=2&SUBJ_ID=SAI0003&CLASS_NO=2&Lang=KOR)

- **수업 목표**
  - 컴퓨팅 사고 : 함수형 프로그래밍언어 스타일
  - 융합 : LLM/ChatGpt를 프로그래밍을 배우는데 활용
  - 글로컬 : Git/GitHub를 통한 협업
  - SW응용 문제해결 능력 : OSS 기본 개념과 도구/ Haskell Programming

- **수업 방법**
  - 플립러닝 방식으로 진행
  - 퀴즈, 요약강의 및 연습문제 풀이
---

## *Week 1-2* — **오픈소스소프트웨어 개요**

> 오픈소스의 역사와 대표적인 사례를 학습

### **오픈소스소프트웨어의 동향**
- [**GitHub Octoverse**](https://octoverse.github.com/)
    - GitHub의 공개 및 오픈 소스 활동을 통해 글로벌 개발자 커뮤니티의 규모 급증
    - 해당 규모 급증에 따라 AI가 어떻게 확장되고 있는지에 대한 내용이 담겨있음

- **최고의 오픈소스 프로젝트**
  1. [Microsoft/vscode](https://github.com/Microsoft/vscode) — 19k
  2. [facebook/react-native](https://github.com/facebook/react-native) — 10k
  3. [tensorflow/tensorflow](https://github.com/tensorflow/tensorflow) — 9.3k
  4. [angular/angular-cli](https://github.com/angular/angular-cli) — 8.8k
  5. [MicrosoftDocs/azure-docs](https://github.com/MicrosoftDocs/azure-docs) — 7.8k
  6. [angular/angular](https://github.com/angular/angular) — 7.6k
  7. [ansible/ansible](https://github.com/ansible/ansible) — 7.5k
  8. [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes) — 6.5k
  9. [npm/npm](https://github.com/npm/npm) — 6.1k
  10. [DefinitelyTyped/DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped) — 6.0k

- **빠르게 성장하고 있는 오픈소스 프로젝트**
  1. [MicrosoftDocs/azure-docs](https://github.com/MicrosoftDocs/azure-docs) — 4.7x
  2. [pytorch/pytorch](https://github.com/pytorch/pytorch) — 2.8x
  3. [godotengine/godot](https://github.com/godotengine/godot) — 2.2x
  4. [nuxt/nuxt.js](https://github.com/nuxt/nuxt.js) — 2.1x
  5. [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) — 2.0x
  6. [wix/react-native-navigation](https://github.com/wix/react-native-navigation) — 1.9x
  7. [spyder-ide/spyder](https://github.com/spyder-ide/spyder) — 1.8x
  8. [tensorflow/models](https://github.com/tensorflow/models) — 1.8x
  9. [home-assistant/home-assistant](https://github.com/home-assistant/home-assistant) — 1.6x
  10. [MarlinFirmware/Marlin](https://github.com/MarlinFirmware/Marlin) — 1.6x

### **오픈소스 소프트웨어란**

- **오픈소스 소프트웨어** : 소프트웨어 저작권가 모든 사람에게 소스코드를 게시, 사용, 복사, 수정 및 배포할 권리를 부여한 소프트웨어
- **OSS License** : 오픈소스 소프트웨어의 사용, 복제, 수정, 배포 권한의 범위를 지정

- **Commercial SW** vs **Open Source SW**
  - Commercial SW (eg. Windows)
    - Individual License(EULA) : 개별 이용 허락
    - Royalty : 로열티 지급
    - Binary only : 실행 바이너리만 제공
    - No reproduction, distribution, modification : 복제, 배포, 수정 불가
    - Limited terms and purposes : 사용기간과 목적 제한
  - Open Source SW
    - Open Source License : 일괄 사전 이용허락
    - No Royalty : 로열티가 없음
    - Source code : 소스코드 제공
    - Reproduction, distribution, modification permitted : 복제, 배포, 수정 허용
    - No limited terms and purposes : 기간, 목적의 제한이 없음
  - Commercial SW와 OSS모두 지적재산권에 의해 보호됨

- **Free SW** vs **Open Source SW**
  - Free Software(자유 소프트웨어)
    - Richard Stallman에 의해 창시됨
    - 공짜(Free of charge)가 아닌 자유(Freedom)을 의미한다.
    - FSF(Free Software Foundation, 1984~)
      - *GPL 1.0 (1989)*
      - *GPL 2.0 (1991)*
      - *GPL 3.0 (2007)*
    - 사용,수정,배포의 자유를 보장하는 소프트웨어
    - Copyleft : 파생 소프트웨어도 자유를 유지해야한다.
  - Open Source Software
    - Eric S. Raymond
      - 오픈소스 개발 문화를 철학적으로 설명
    - OSI(Open Source Initiative, 1998~)
      - 'Free'의 모호함 해결 -> 공개된 코드에 초점을 맞춤
      - OSS와 Closed Source SW의 결합
      - 법적 Licence가 명확하다.

### **오픈소스 소프트웨어 License**
| Licenses | Linked with Proprietary SW | Must publish Modification | Patent Protection |
|:--------:|:--------------------------:|:-------------------------:|:-----------------:|
| GPK 2.0 | X | O | X |
| LGPL | O | O | X |
| MIT / BSD | O | X | X |
| Apache 2.0 / MPL1.0,1.1 | O | O | O |
- Linked with Proprietary SW : 상용 소프트웨어와의 연동
- Must publish Modification : 수정 시 공개 의무
- Patent Protection : 특허 보호 조항

---

## *Week 2-1* — **버전 관리 개요**

- **버전 제어 시스템이 없을경우**
  - 백업 사본을 만든다.
  - 버전 번호나 날짜를 추가한다.
  - 협업을 위해 공유 폴더를 사용한다.

### **VCS (Version Control System)**
- 시간 경과에 따른 파일 추적을 통해 이전 작업으로 쉽게 돌아갈 수 있다.
- VCS Software
  - *CVS (Concurrent Version System)*
  - *SVN (Subversion)*
  - *Mercurial*
  - *Darcs*
  - *Git*
- Repository (저장소)

### **VCS에서 버전 관리**
- VCS에서 버전 관리는 Main Trunk위에서 이루어진다.
  - Trunk -> branch in Git
- **Checkin**
  - 파일을 checkin하고 시간이 지남에 따라 수정
  - commit in Git
- **Checkout** and editing
  - 파일을 checkout하여 편집한 후 다시 checking 한다.
  - fetch/pull in Git
- **Diffs**
  - trunk(branch)에 파일이 진행됨에 따라 변경된 내역이 저장된다.
- **Branching**
  - 변경 사항에 대한 기록을 보관 가능하도록 별도의 폴더에 복사한다.
- **Merging**
  - 한 브랜치에서 다른 브랜치로 변경 사항을 병합한다.
- **Conflicts**
  - 병합 과정에서 변경 사하이 겹치는 경우 발생한다.
  - 프로젝트 개발 의도에 따라 해결 방법이 달라진다.
- **Tagging**
  - 모든 개정판에 태그를 지정하여 버전 관리를 할 수 있다.

### **VCS의 주요 유형**
- **Centralized VCS**
  - 중앙 서버의 history 관리
  - 여러 사용자가 있는 하나의 중앙 저장소
  - *eg. CVS, SVN*
- **Decentralized(Distributed) VCS**
  - 중앙 서버가 없이 history 관리
  - 모든 사용자가 자신의 로컬 저장소를 소유한다 (분산)
  - 별도의 중앙 원격 저장소가 존재
  - fork, pull을 요구
  - *eg. GIT, Mercurial, Darcs*
---

## *Week 2-2* — **Git**

> Git의 기본 명령어와 commit 흐름 익히기

### **Git의 기본 구조**
- Git에서의 분산 제어 시스템
  - Workspace : 작업 중인 파일
  - Index : version이 없는 임시 파일
    - 다음 커밋에서 고려될 파일
  - Local Repository : 로컬 저장소에서 commit된 파일
  - Remote Repository : 로컬에서 원격으로 push된 파일

### **Git의 작업흐름**
- ![Git](data:image/png;base64,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)
- `git add` : Workspace에서 변경된 파일을 Index영억으로 옮기는 명렁어
- `git commit` : Index영역의 내용을 Local Repository에 기록하는 명령어
  - `-a option` : git add없이 수정된 파일 전체를 한번에 커밋
    - 이미 추적중인 file만 가능하다.
  - `-m option` : 커밋 시 커밋내용을 넣을 수 있음
- `git push` : Local Repository의 commit을 Remote Repository로 업로드하는 명령어
- `git fetch` : Remote Repository의 변경내역을 Local Repository의 remote-tracking branch로 가져와 갱신하는 명령어
  - 자동으로 merge되진 않는다.
- `git merge` : 다른 브랜치를 현재 브랜치와 병합시키는 명령어
- `git pull` : git fetch + merge
- `git diff` : Workspace와 Index영역의 파일의 차이를 확인하는 명령어
  - `HEAD option` : 가장 최근 Commit과의 차이를 확인하는 명령어
- `git clone` : Remote Repository에 있는 프로젝트를 Local 환경에 가져오는 명령어
---

## *Week 2-3* — **GitHub, Fork, Pull Request**

- **[GitHub](https://github.com/)** : Git 기반 소스 코드 호스팅을 하는 사이트
  - 포크, 풀 리퀘스트, 코드 검토 기능등을 지원한다.

-![fork, pr](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ0LoGaVqwD-sKnhpfG9U54meIglH-r_zfmEw&s)
- `fork` : GitHub의 다른 사람의 Remote Repository를 나의 Remote Repository로 복제
- `pull request(PR)` : 나의 Remote Repository에서 수정한 내용을 원래 프로젝트에 반영해달라 요청
---

## *Week 2-4* — **Git: Advanced Topics**

> Git의 commit 수정, branch merging, rebase, blame 추적등을 학습

- commit 수정 : `git commit --amend`
  - 가장 마지막 commit의 내용을 수정할 수 있는 명령어
  - 수정시 local과 remote에서의 commit의 불일치로 push가 거부된다.
    - git push --force를 하여 강제로 커밋을 덮어쓴다.
- add 취소 : `git reset`
  - staging된 파일을 unstaged 상태로 되돌리는 명령어
- commit 제거 : `git reset HEAD~1`
  - 최근 commit을 하나 이전 상태로 되돌린다 -> 마지막 커밋 삭제
- branch 병합 : `git merge`
  - 두 branch의 이력들을 병합하는 명령어
    - 병합시 conflict가 일어날 수 있으므로 주의해야한다.
- 기록 재정렬 : `git rebase`
  - branch의 커밋들을 다른 branch의 최신 커밋 뒤로 옮기는 명령어
  - VS merge
    - merge : 기존 이력 그대로 유지 -> 브랜치를 합친 흔적이 존재
    - rebase : 커밋 이력을 새로 작성 -> history가 깔끔해짐
- 중간 커밋 수정 : `git rebase -i`
  - 특정 커밋을 골라 주성하는 명령어
- 추적 : `git blame`
  - 파일의 각 줄이 누가 언제 수정했는지 추적
  - 각 줄마다 수정자와 커밋 ID가 표시된다.

---

## *Week 3* — **Markdown**

> README.md, Wiki, Documentation 등에서의 활용
> *이탤릭체*, **굵은 글씨**, `코드 블록`, 링크, 이미지 삽입 등을 학습

### **Markdown**

- 일반 텍스트 편집기를 사용하여 서식이 지정된 텍스트를 생성하기 위한 가벼운 언어
- John Gruber, Aaron Swartz에 의해 만들어짐
- GitHub에서 `README.md` 파일에서 사용된다

### **제목 및 구분선**

- `=====` : =줄은 HTML의 `<h1>`과 같은 의미를 지닌다 → 가장 큰 제목
- `--------` : -줄은 HTML의 `<h2>`와 같은 의미를 지닌다 → 중간 크기의 제목
- `#` 개수에 따라 제목 수준이 달라진다
    - `#` → `<h1>`
    - `##` → `<h2>`
    - `###` → `<h3>`
- 문단은 빈 줄로 구분이 된다
    - Markdown에선 줄 바꿈이 없을 시 하나의 문단으로 합쳐진다
    - 한 줄의 끝에 공백 두 개를 넣을 시 줄이 바뀐다 → `<br>` 태그와 같은 역할

### **기울임꼴, 굵은꼴 등**

- `_text_` : _(언더스코어)로 감싸면 기울임이 들어간 italic체로 바뀐다.
- `**text**` : **로 감싸면 굵은 bold체로 표시된다.
- `` `text` `` : (backtick)으로 감싸면 코드나 명령어처럼 고정폭 폰트가 된다.
- `---`, `***`, `___` : 수평 구분선이 생성된다.

### **글머리 기호와 숫자가 있는 목록**

- **`1.`, `2.`** : 번호 있는 순서 목록(ordered list)을 만든다.
    - 자동으로 1, 2, 3 순으로 넘버링됨.
- `*`, `-`, `+` : 기호를 사용해 불릿 목록(bullet list)을 만든다.
    - 별표(`*`), 대시(`-`), 플러스(`+`) 모두 가능함.
- 들여쓰기 (space 2칸 이상) : 앞에 공백 2칸 이상을 주면 중첩으로 인식된다.
    - 순서 목록 안에 불릿 목록을 넣을 때 사용.

### **링크 및 이미지**
- `[text](URL)` : 링크를 만드는 문법.
    - `[표시될글자](연결할주소)` 형태로 작성.
- `![alt](이미지경로 "제목")` : 이미지를 삽입하는 문법.
    - 느낌표 `!` 뒤에 대괄호(`[]`)와 소괄호(`()`)를 사용.
    - 대괄호 안: 이미지의 대체 텍스트(alt)
    - 소괄호 안: 이미지 파일 경로
    - 따옴표 안: 툴팁으로 표시될 제목
- `>` : 인용문(quote) 문법.
    - 줄 앞에 `>`를 붙이면 블록 인용문이 만들어진다.
    - 여러 문단을 인용하려면 각 문단마다 `>`를 붙여야 한다.
- `<abbr title="...">텍스트</abbr>` : HTML 문법을 직접 사용하는 예시.
    - 마크다운 안에서도 일부 HTML 태그(`<abbr>`, `<br>`, `<sub>` 등)는 그대로 인식된다.

### **Editor**

- **VS Code**
    - `Ctrl + Shift + V` : 작성한 Markdown 문서를 미리보기 가능

---