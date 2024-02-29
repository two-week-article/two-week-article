# two-week-article

_큰 주제를 가지고 2주 동안 관심있는 소주제의 article을 작성합니다._ 

## Contributors
<hr/>

_첫 글을 작성하면 contributors로 추가 됩니다._

<a href="https://github.com/two-week-article/two-week-article/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=two-week-article/two-week-article" />
</a>

<br/>
<br/>

## 목차

1. [article 작성 전 준비](#article-작성-전-준비)
- [작성자 등록하기](#작성자-등록하기)
- [로컬에서 실행시켜 포스트 작성 현황 확인하기](#로컬에서-실행시켜-포스트-작성-현황-확인하기)
- [article 작성하기](#article-작성하기)

<br/>
<br/>

## article 작성 전 준비
<hr/>

### 작성자 등록하기

/two-week-article/_data/authors.yml 파일에 들어갑니다.

아래 코드블럭을 복사한 후 수정해 한줄 띄워 붙혀넣기 해주세요!<br/>

```console
{author_id}:
   name: {full name}
   twitter: {twitter_of_author}
   url: {homepage_of_author}
```

- author_id는 고유한 키값입니다.
{}까지 모두 지워주신 후 다른 사람과 겹치지 않도록 편하게 정해주시면 됩니다.

- name은 실제로 표시되는 작성자명 입니다.
닉네임이나 실명을 적어주시면 되며, 한글 영어 상관없습니다.

- twitter는 가지고있다면 twitter 닉네임을 적어주시면 됩니다.

- url은 개인 블로그 또는 홈페이지로 연결됩니다.
깃허브 주소도 좋습니다.

<br/>
<br/>


### 로컬에서 실행시켜 포스트 작성 현황 확인하기

저희는 [Jekyll(지킬)](https://ko.wikipedia.org/wiki/%EC%A7%80%ED%82%AC_(%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4))을 사용하여 정적 사이트를 만들었습니다.

아래 명령어를 루트 디렉토리에서 터미널에 입력해 실행시킬 수 있습니다.

```console
bundle exec jekyll s
```

초기 주소값은 http://127.0.0.1:4000/ 입니다.<br/>
혹시 4000번 포트를 사용하는 다른 프로그램이 있다면 포트 변경이 필요합니다.

<br/>
<br/>

### article 작성하기

article을 작성하기 위해서는 .md 파일에 대해 알 필요가 있습니다.

[MD(Markdown) 파일 형식](https://kb.fileformat.app/ko/extension/md-file-info/)은 개발자 John Gruber와 Aaron Swartz가 2004년에 만들었습니다. HTML로 변환할 수 있는 가볍고 읽기 쉽고 쓰기 쉬운 일반 텍스트 형식으로 설계되었습니다.

먼저 /two-week-article/_posts 폴더에 파일을 하나 만듭니다.<br/>
파일의 양식은 <span style='color: red'>yyyy-mm-dd-큰주제-소주제-작성자.md</span>로 통일하도록 하겠습니다.

파일명을 작성하실때는 영어로 작성하시는 것을 추천합니다.<br/>
깃허브에서는 한글 파일명을 지원하지 않기 때문에 한글 깨짐현상이 있습니다.<br/>
해결하는 방법[(링크)](https://velog.io/@im-yeobi/git-%ED%95%9C%EA%B8%80-%ED%8C%8C%EC%9D%BC%EB%AA%85-%EA%B9%A8%EC%A7%90-%ED%95%B4%EA%B2%B0)가 있지만 저희는 생략하기로 합니다.

파일을 만들었다면 파일을 열어주세요!

상단에 다음과 같은 양식을 먼저 입력 해주세요.

```console
---
title: 
author: 
date: 2024-02-26 21:07:00 +0900
categories: [대분류, 소분류]
tags: [대주제]
---
```

- title은 제목을 입력하는 곳입니다.
제목의 언어와 이모지사용은 상관없습니다. 저희는 유니코드(UTF-8)을 사용합니다.
다만 제목에서 []를 사용하는 경우 배열로 인식하여 문자열로 만들어주기 위해 ''를 씌워주세요.

- 작성자는 위에 _작성자 등록하기_ 에서 작성하신 고유한 키값을 입력해주세요.

- date는 한국 시간을 적용하기 위하여 +0900을 넣어주세요!

- categories는 대분류와 소분류를 나누려고 합니다.
대분류와 소분류는 조금 더 논의하여 정확하게 나누었으면 해요!

- tags는 2주간격으로 변하는 주제를 적습니다.


구체적인 작성법은 Jekyll 테마를 만드신 chirpy의 블로그[(링크)](https://chirpy.cotes.page/posts/text-and-typography/)를 참고해주세요!

