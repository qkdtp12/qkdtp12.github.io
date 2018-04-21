---
layout: post
title:  "How to start Jekyll!"
date:   2018-04-17 15:01:27 +0900
categories: jekyll start windows
---

> <https://jekyllrb.com/>

Jekyll은 여러 형태의 텍스트와 소스들로 구성 정적 파일들을 웹사이트로 생성시켜주는 툴입니다.<br>
Github Pages 를 통해서 정적 페이지로 무료 블로그를 만들고 사용할 수 있습니다.<br>

Jekyll 설치하기
-------------

### 준비물

* Ruby
* RubyGem
* Python 2.7

Jekyll은 공식적으로 Windows 운영체제를 지원하지 않지만 실행할 수는 있습니다.

1. Ruby를 설치합니다.

> <https://rubyinstaller.org/downloads/>

![install ruby]({{site.url}}/assets/jekyll/ruby1.png)

> Add Ruby executables to your PATH 를 체크하여 환경 변수에 추가합니다.

![install option]({{site.url}}/assets/jekyll/ruby2.jpg)
   
2. Python을 설치합니다.

> <https://www.python.org/downloads/>

Python2.7을 설치합니다.

> 환경 변수를 추가합니다.

C:\Python27;C:\Python27\Scripts;

![python path]({{site.url}}/assets/jekyll/python1.png)
    
3. Gem 명령어를 통해서 Jekyll 를 설치합니다.

`gem install jekyll`

> 회사와 같은 환경에서 인증서 문제로 https 저장소에 접근이 안되는 경우
    
`gem source -r https://rubygems.org/`<br>

`gem source –a http://rubygems.org/`

4. Jekyll을 시작합니다.

[python2.7]: https://www.python.org/downloads/
[tale-github]: https://github.com/chesterhow/tale
[jekyll-kor]: http://jekyllrb-ko.github.io/
[reference-site]: http://tech.whatap.io/2015/09/11/install-jekyll-on-windows/
[markdown]: https://gist.github.com/ihoneymon/652be052a0727ad59601