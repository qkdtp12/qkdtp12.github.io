---
layout: post
title: "How to start Jekyll!"
date: 2018-04-17 15:01:27 +0900
comments: true
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
   
2. Python2.7을 설치합니다.

    > <https://www.python.org/downloads/>
    
    > 환경 변수를 추가합니다.
    
    C:\Python27;C:\Python27\Scripts;
    
    ![python path]({{site.url}}/assets/jekyll/python1.png)
    
3. Gem 명령어를 통해서 Jekyll 를 설치합니다.

    `gem install jekyll`

    > 회사와 같은 환경에서 인증서 문제로 https 저장소에 접근이 안되는 경우
    
    `gem source -r https://rubygems.org/`<br>

    `gem source –a http://rubygems.org/`

4. Jekyll을 시작합니다.

    jekyll 폴더를 만들어 줍니다.
    
    `mkdir C:\jekyll`
    
    폴더로 이동하여 jekyll을 실행합니다.
    
    `jekyll serve`
    
    ![jekyll serve]({{site.url}}/assets/jekyll/jekyll1.jpg)
   
    wdm을 설치하라고 합니다.wdm을 설치합니다.
    
    `gem install wdm`
    
    다시 jekyll을 실행합니다.
    
    `jekyll serve`
    
    브라우저를 통해 localhost:4000에 연결합니다.
    
    `http://localhost:4000`
    
    ![jekyll serve]({{site.url}}/assets/jekyll/jekyll2.jpg)

5. Jekyll 사이트를 생성합니다.
        
    `jekyll new C:\jekyll\blog`
    
    ![jekyll serve]({{site.url}}/assets/jekyll/jekyll3.jpg)
        
    새로 생성된 프로젝트의 Gemfile을 bundler를 통해서 설치하기 위해서 bundler를 설치합니다.
    
    `gem install bundler`
    
    생성한 blog 폴더로 이동하여 bundle 명령어를 실행합니다.
    
    `cd blog`
    
    `bundle`
    
    Jekyll을 실행합니다.
    
    `jekyll serve`
    
    실행된 화면을 확인합니다.
    
    ![jekyll serve]({{site.url}}/assets/jekyll/jekyll4.jpg)
    
[python2.7]: https://www.python.org/downloads/
[tale-github]: https://github.com/chesterhow/tale
[jekyll-kor]: http://jekyllrb-ko.github.io/
[reference-site]: http://tech.whatap.io/2015/09/11/install-jekyll-on-windows/
[markdown]: https://gist.github.com/ihoneymon/652be052a0727ad59601