# LaTeX 문서 작성법 이해 
---

## Latex 작성법  

latex으로 조판하는 법은 대학교에 와서 word 등을 사용하고 한글을 사용하던 사람 입장에서는 조금 굳이라는 생각을 들게 만드는 것일 수도 있다.  
[플로우차트](https://flowchart.fun)같은 경우 일반적으로 자주 그릴 수 있는 것이다. 플로우차트와 다양한 다이어그램을 그렸다. 다이어그램으로 일반적으로 어떻게 작성하고 어디서 멈춰야할지 판단해야한다. 

경제학과로써는 TeX의 조판과정을 완벽히 이해하고 어떻게 코드들이 조판을 해가는지에 대해서는 몰라도 상관은 없다. 과제물로 자주 나오는 수식과 그래프도 가득한 유인물들과 책들이 대부분 LaTeX으로 조판되었으니 우리는 그저 LaTeX을 사용해서 문서를 작성해서 과제로 업로드 하는 것이 중요하다. 

LaTeX는 특히 수학, 과학 및 공학 분야에서 고품질 문서를 ​​만드는 데 사용되는 조판 언어로 텍스트, 방정식 및 그림의 레이아웃과 서식을 정밀하게 제어할 수 있다.
 LaTeX를 작성하려면 TeXstudio 또는 Overleaf와 같은 텍스트 편집기를 사용할 수 있다. 로컬에서 하고싶지 않는 경우 온라인 편집기 중 가장 유명한 Overleaf를 사용하는 것이 편하다. 한국어를 지원하긴 하지만 대부분 영어로 쓰는 것이 도움이 된다. 한국어를 쓰고 싶다면 [권현우](https://willkwon-math.github.io/)교수님의 laTeX 작성법에 대해서 듣길 바란다. 한국어로 작성되어 있는 아주 좋은 강의들과 피피티를 공개해주셔다. 또한 [카이스트의 laTeX강의](https://youtu.be/6pTvBP8t58c) 또한 도움이 될 것이다. 

LaTeX 코드는 PDF 문서로 컴파일된다. overleaf에 이런 자습서들이 많으니 가서 참고하면 좋다. 


## [Overleaf](https://www.overleaf.com/learn)로 하는 LaTeX 작성법

LaTeX를 작성할 때 언어의 구문과 구조를 염두에 두는 것이 중요합니다. 예를 들어 방정식은 일반적으로 달러 기호($$)로 묶고 명령은 백슬래시(\)로 시작합니다. 들여쓰기와 공백을 사용하여 코드의 가독성을 높이는 등 코드 형식에 주의를 기울이는 것도 중요합니다.

LaTeX 사용의 이점 중 하나는 전문가 수준의 문서를 쉽게 작성할 수 있다는 것입니다. 이는 특히 학술 논문, 프리젠테이션 및 보고서에 유용합니다. LaTeX는 또한 복잡한 수학 방정식과 기호를 생성할 수 있어 과학계에서 널리 사용됩니다.

언어의 기능을 확장할 수 있는 많은 LaTeX 패키지가 있습니다. 이러한 패키지는 그래픽을 포함한 테이블 생성 및 참고 문헌 서식 지정과 같은 다양한 목적으로 사용할 수 있습니다.(우리가 쓸 Pgfplot and tkiz ,amsmath... etc.)

전반적으로 LaTeX는 서식 및 레이아웃을 정밀하게 제어하여 고품질 문서를 ​​작성하기 위한 강력한 도구입니다. 연습과 인내를 통해 누구나 LaTeX 작성법을 배우고 전문가 수준의 문서를 생성할 수 있습니다.
LaTeX는 과학 문서에 특히 유용하지만 이력서, 편지, 심지어 소설을 포함한 모든 유형의 문서에 사용할 수 있습니다.

나중에는 beamer 라는 패키지를 사용해 피피티로 바로 변환하여 발표할 수 있다. 


## overleaf 및 tex 조판의 이해  

overleaf 로 쓴 코드는 같은 이름의 tex 파일로 올라가니 그것을 참고하면 된다. 아래 단락부터는 명령어들에 대한 것들을 주로 다룬다. 직접 실습할 때에는 아무 경제학 교재 1장의 내용을 따라 작성해보는 것도 도움이 된다.  
아래는 한국어 버전이 아닌 영어버전을 기준으로 하였으나 권현우 선생님의 글을 보면 obilivior 나 kotex 패키지를 통해 한국어를 사용할 수 있게 되어있으나 가능한 한 영어 공부와 함께 영어로 작성하는 것을 추천한다.  


```{LaTeX}
\\\\documentclass{article}

\\\\title{Economic Report}
\\\\author{Your Name}

\\\\begin{document}

\\\\maketitle

\\\\section{Introduction}

Here is where you would provide a general statement about the importance of the topic or problem you are addressing. You should also provide background information about the topic to give context to your report. Clearly state the main question or problem you are addressing in the report, and provide an overview of the structure of the report, including what you will cover in each section.

\\\\section{Methodology}

In this section, you should describe the methods you used to conduct your research. For example, you might describe the data sources you used, the statistical analyses you performed, or the survey questions you asked.

\\\\section{Results}

Here is where you would present the results of your research. You might include tables or graphs to help illustrate your findings.

\\\\section{Discussion}

In this section, you should interpret your findings and discuss their implications. You might also discuss the limitations of your research and suggest areas for future research.

\\\\section{Conclusion}

Finally, you should summarize your findings and conclusions, and suggest any implications for policy or practice.

\\\\end{document}

```

`\section{단원}` 으로 작성하면 오른쪽 하단에 그 단원들이 표기되고 관련된 내용을 적으면 된다. 경제학보고서의 형태는 국책 보고를 읽거나 하면된다. 

또한 이미지 포함을 위한 `\usepackage{graphicx}` 또는 목차 생성을 위한 `\tableofcontents`와 같은 필요한 LaTeX 패키지 및 명령을 포함해야 한다.

## tkiz 패키지로 그림 그리기  
pgfplot 패키지와 tkiz 패키지를 통해서 그래프와 수식에 대한 설명 및 균형점을 그려넣을 수 있다. 

현재 지금 보고 있는 이 마크다운 문서에서도 latex 코드 를 작성하여 집어넣을 수는 있으나 그래프나 그림을 바로 넣을 수는 없다.  

Overleaf LaTeX 컴파일러를 사용하여 별도로 그래프를 생성한 후에 그 이미지를 저장하고 . 그래프를 생성한 후에는 `![alt text](image_path)` 구문을 사용하여 Markdown 문서에 이미지로 그래프를 포함할 수 있습니다.

```
\\documentclass{article}
\\usepackage{tikz}

\\begin{document}

\\begin{tikzpicture}
\\draw[->] (0,0) -- (10,0) node[right] {Year};
\\draw[->] (0,0) -- (0,6) node[above] {GDP (in trillions of dollars)};
\\draw[help lines] (0,0) grid (9,5);
\\foreach \\x in {1,2,...,9} \\draw (\\x,0) node[below] {$\\x$};
\\foreach \\y in {1,2,...,5} \\draw (0,\\y) node[left] {$\\y$};
\\draw[blue, thick] (1,1) -- (2,1.5) -- (3,2.5) -- (4,3) -- (5,3.5) -- (6,4) -- (7,4.5) -- (8,5) -- (9,5.5);
\\end{tikzpicture}

\\end{document}

```
위의 코드를 가지고 이미지를 뽑으면 마크다운에 입력할 때는 그 그래프 png 파일을 아래와 함께 작성해서 넣으면 된다. 

```
![Graph of GDP over time.](path/to/image.png)

```


## LateX을 이용한 보고서 작성법  참고용 링크 

https://www.overleaf.com/learn/latex/Subscripts_and_superscripts
https://texample.net/tikz/examples/area/economics/
[Basic LaTeX Example for Economics Writing](https://www.youtube.com/watch?v%3DAMZSL9yiRr8)
[Applied LATEX for Economists, Social Scientists and Others 2014](https://www.tcd.ie/Economics/TEP/2014/TEP0214.pdf)
[pgfplot to make economic graphs in latex](https://towardsdatascience.com/using-pgfplots-to-make-economic-graphs-in-latex-bcdc8e27c0eb)
[Help with economics graph](https://tex.stackexchange.com/questions/449304/help-with-economics-graph)
[usepackage{TikZ } for economists](http://static.latexstudio.net/wp-content/uploads/2016/06/tikzforeconomists-110619150244-phpapp01.pdf)
[latex tempelete for economist](https://github.com/talgross-bu/Template-for-Overleaf)