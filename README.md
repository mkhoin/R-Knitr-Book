## R과 Knitr를 활용한 데이터 연동형 문서 만들기 예제 코드##

### 버전업에 대하여 

#### RStudio, rmarkdown(R markdown version 2) 환경에서 작업하기 

- `R markdown`이 버전업이 되면서 `rmarkdown`이 되었고, RStudio 0.98 버전부터는 기본적으로 `rmarkdown`을 사용하여 문서 작업을 할 수 있도록 환경이 바뀌었다. [rmarkdown 사이트](http://rmarkdown.rstudio.co)에관련된 정보를 확인할 필요가 있다. 

    - 가장 큰 차이점은 `팬독`(http://johnmacfarlane.net/pandoc/) 마크다운을 사용한다는 점이다. 따라서, 팬독  사이트에서 팬독을 별도로 컴퓨터에 설치할 필요가 있다. 팬독 마크다운은 문서의 표현력이 높고, 다양한 포맷으로 문서를 전환시키는데 정말 놀라운 기능을 가지고 있다. 


    - `rmarkdown`은 아직(2014년 7월 8일부) CRAN에 등재되어 있지 않다. 따라서, 아래와 같은 코드를 R콘솔에서 실행하여 깃허브를 통해 설치한다. `devtools`라는 패키지가 설치되어 있지 않은 경우라면 `install.packages("devtool")`를 싫행하여 설치한다.

        ~~~~
            devtools::install_github("rstudio/rmarkdown")
        ~~~~

    - 또, Rmd 문서 내부에서 `YAML 사전정의부`(YAML front matter)를 사용한다는 점도 크게 달라진 부분이다. 윈도우즈 사용자라면 `YAML 사전정의부`에서 설정을 잡을 때 한글과 관련된 부분에서문제가 있을 수 있는데, 이와 관련해서는 아래를 참고한다. 


> 원도우즈 환경에서 RStudio 사용시 고려할 부분

> 원도우즈에서 RStudio에서 rmakdown을 사용할 때 생기는 문제를 완전하지는 않지만 다음과 같이 해 보는 것도 괜찮다.

> - [rmakdown, Rsutiod, Windows 사용시 한글 사용의 문제](http://ksbapp.com/WindowsKorean.html)

### 예제 코드 사용법

- 2 장 '필요한 오픈소스 프로그램 설치'에 따라 설치한 R과 RStudio에서 코드를 실행한다고 하는 것을 기준으로 했다.
 
- 특정 R 패키지가 필요한 경우에 컴퓨터에 설치되어 있지 않다면 오류를 보낸다. 이런 경우에는 해당 패키지를 책의 2장에서 설명한 대로 설치한 다음 실행하면 된다.  

- 책에 있는 그대로의 코드를 옮기는 의미가 없다고 생각했기 때문에, 책의 내용을 매뉴얼로 정리하는 형태가 많다. 


### 다운로드 ###

- 이 화면의 오른쪽을 보면 `Download ZIP`이라고 하는 단추가 있다. 이 단추를 누르면 전체 내용이 다운로드된다. 

### 다운로드후 사용 ###

- 각각의 폴더는 RStudio 프로젝트로 구성되어 있다. 따라서, 각 폴더에는 확장자가 `.Rproj`라고 되어 있는 파일이 있는데, 이 파일을 클릭하면 RStudio가 해당 디렉터리를 워킹디렉터리로 설정하면서 열린다. 

- 각 폴더에는 `chapterIntro.md`라는 사용법을 간단하게 소개한 파일을 있다. 꼭 확인하고 자료들을 확인하기를 권한다. 


### Shiny 업데이트와 관련된 내용 추가

이 책은 `shiny` 패키지를 주요 챕터로 다루고 있는데,최근에 버전이 1.0으로 향상되어 이에 대해 별도로 정리하였다. 

- [샤이니의 기초](http://ksbapp.com/ShinyBasic.html)

- [샤이니 앱 작성을 위한 기본 테크닉](http://ksbapp.com/BasicTechniques.html)

- [샤이니 앱 꾸미기(레이아웃)](http://ksbapp.com/shinyLayout.html)

- [샤이니 반응성](http://ksbapp.com/shinyReactivity.html)

- [샤이니 앱에서 파일, 이미지 업로딩과 다운로딩](http://ksbapp.com/FileNImage.html)

- [샤이니를 이용한 인터랙티브 문서](http://ksbapp.com/shinyInRmd.html)

[샤이니 웹 사이트](http://shiny.rstudio.com/articles/cheatsheet.html) 에서  놀랍도록 잘 정리된 cheat sheet를 제공하고 있다.
