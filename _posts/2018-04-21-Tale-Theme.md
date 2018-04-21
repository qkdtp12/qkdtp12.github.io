---
layout: post
title: "Install Tale theme on Jekyll"
date: 2018-04-21 22:01:27 +0900
comments: true
categories: Install Tale theme
---

## Tale 테마

Jekyll을 설치하면 아래와 같은 화면을 확인할 수 있습니다. 저는 마음에 들지 않네요. :)

> Jekyll 설치는 이전 포스트를 참고하세요.{{ site.baseurl }}{% post_url 2018-04-21-how-to-start-jekyll %}

![default them,e]({{site.url}}/assets/tale/jekyll.jpg)

> <https://github.com/chesterhow/tale>

심플한 테마인 Tale로 Jekyll의 화면을 바꿔보도록 하겠습니다.

## 기능
- Easy installation
- Compatible with GitHub Pages
- Responsive design (looks just as good on mobile)
- Syntax highlighting, with the help of Pygments
- Markdown and HTML text formatting
- Pagination of posts

## 설치

### Local - Ruby Gem method

1. `Gemfile`에 아래 명렁어를 추가합니다.

```ruby
gem "tale"
```

2. bundle  명령어를 통해서 설치합니다.

```ruby
$bundle
```

3. `_config.yml`에 아래 명령어를 추가합니다.

```yaml
theme:      tale

permalink:  /:year-:month-:day/:title
paginate:   5
```

다른 `theme:` 옵션은 제거합니다.

4. `index.md` 를 `index.html`로 변경합니다.

5. `about.md` 의 `layout:` 을 `post`로 변경합니다.

```Markdown
layout: post
```

### Github Page - github.io

1. `Gemfile`에 아래 명렁어를 추가합니다.

```ruby
gem "jekyll-remote-theme"
gem "jekyll-paginate"
```

2. bundle  명령어를 통해서 설치합니다.

```ruby
$bundle
```

3. `_config.yml`에 아래 명령어를 추가합니다.

```yaml
remote_theme: chesterhow/tale

permalink:    /:year-:month-:day/:title
paginate:     5

plugins:
  - jekyll-paginate
  - jekyll-remote-theme
```

다른 `theme:` 옵션은 제거합니다.

4. `index.md` 를 `index.html`로 변경합니다.

5. `about.md` 의 `layout:` 을 `post`로 변경합니다.

### 사용

빌드하고 사이트에 적용하려면 아래 명령어를 실행하세요.

```bash
$ bundle exec jekyll serve
```

> <http://localhost:4000>

![tale them,e]({{site.url}}/assets/tale/tale.jpg)

Tale 테마가 적용된 화면을 볼 수 있습니다.(local)
Github를 통해서 서비스된 화면은 본 사이트를 참고해 주세요.