---
layout: post
author: SOYOU
title: "Sequence Diagram을 스크립트로 그리자"
tags: Mac 자동화 PlantUML SequenceDiagram VSCode Marxico
---
<div id='preview-contents' class='note-content'>
    <div>
        <div class="toc">
            <div class="toc">
                <ul>
                    <li><a href="#plantuml">PlantUML</a></li>
                    <li><a href="#visual-studio-code">Visual Studio Code</a>
                        <ul>
                            <li><a href="#step-1">step 1</a></li>
                            <li><a href="#step-2">step 2</a></li>
                            <li><a href="#step-3">step 3</a></li>
                            <li><a href="#step-4">step 4</a></li>
                            <li><a href="#step-5">step 5</a></li>
                            <li><a href="#다이어그램-png">다이어그램 -&gt; PNG</a></li>
                        </ul>
                    </li>
                    <li><a href="#후기">후기</a></li>
                </ul>
            </div>
        </div>
    </div>

    <h1 id="plantuml">PlantUML</h1>

    <p>이전에 PlantUML을 이용해서 시퀀스 다이어그램을 스크립트로 그려보았던 기억이 있습니다. <br>
        애플 로그인 개발을 진행하다가 다이어그램을 그려봐야 할것 같아서 찾아보았습니다.</p>

    <p><a href="https://plantuml.com/ko/" target="_blank">PlantUML</a> 홈페이지를 보니 <br>
        <a href="https://plantuml.com/plantuml/" target="_blank">Online Server</a> 를 통해서 웹에서 바로 작성이 가능하고 <br>
        다이어그램도 바로 확인할 수가 있어서 좋았습니다.
    </p>

    <p><strong>하지만</strong> </p>

    <p><img longdesc="https://d.pr/i/RVQPEE+" alt="" title="" type="image/jpeg" src="https://d.pr/i/RVQPEE+" class=""> <br>
        1번, 2번 영역의 광고가 스크립트 작성을 상당히 방해합니다. <br>
        Sumit 클릭 때마다 새로고침으로 깜빡이며 <br>
        2번 영역에는 비디오 광고가 자동으로 재생까지 되어서 <br>
        살살 약이 오르게 됩니다.</p>

    <p>그래서 다른 방법을 찾아보았고, <br>
        제가 선택한 방법을 공유하고자 합니다.</p>

    <h1 id="visual-studio-code">Visual Studio Code</h1>

    <p>갑자기 Visual Studio Code 에디터가 나온 이유로는 <br>
        <a href="https://plantuml.com/ko/running" target="_blank">PlantUML 사용하기</a>에서 플러그인을 발견하기도 했고 <br>
        평소 제가 한번 써보고 싶었던 에디터 였는데 <br>
        딱히 사용할 명분(?)이 없었기에 <br>
        이번 기회에 시퀀스 다이어그램 전용 편집기로 사용해 보려고 합니다.
    </p>

    <p><a href="https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml" target="_blank">PlantUML VSCode Plugin 페이지</a>에 자세한 설명이 있습니다. <br>
        저는 MacOS를 사용중에 있기 때문에 Mac에서 제가 진행한 순서를 작성해 보았습니다.</p>

    <h2 id="step-1">step 1</h2>

    <p><a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a> 다운로드 후 설치합니다.</p>

    <h2 id="step-2">step 2</h2>

    <p><img longdesc="https://d.pr/i/IG61Ey+" alt="" title="" type="image/jpeg" src="https://d.pr/i/IG61Ey+" class=""> <br>
        Visual Studio Code를 실행 후 <br>
        <code>COMMAND + P</code>로 패널을 열고 <br>
        <code>ext install plantuml</code>를 입력합니다.
    </p>

    <h2 id="step-3">step 3</h2>

    <p><img longdesc="https://d.pr/i/gj6geP+" alt="" title="" type="image/jpeg" src="https://d.pr/i/gj6geP+" class=""> <br>
        1번 개발자 ‘jebbs’를 확인 후, <br>
        2번을 클릭해서 설치합니다.</p>

    <h2 id="step-4">step 4</h2>

    <p><img longdesc="https://d.pr/i/UXxcHD+" alt="" title="" type="image/jpeg" src="https://d.pr/i/UXxcHD+" class=""> <br>
        <code>COMMAND + N</code>로 새파일을 연후에 우측 하단의 ‘Plain Text’를 클릭하면 <br>
        언어 모드를 선택할 수 있습니다. 여기서 ‘Diagram’을 선택합니다.
    </p>

    <h2 id="step-5">step 5</h2>

    <p><img longdesc="https://d.pr/i/7Fry6x+" alt="" title="" type="image/jpeg" src="https://d.pr/i/7Fry6x+" class=""> <br>
        시퀀스 다이어그램 스크립트를 입력 후 <br>
        <code>ALT + D</code> 단축키를 통해서 우측에 미리보기 화면을 불러낼 수 있습니다.
    </p>

    <h2 id="다이어그램-png">다이어그램 -&gt; PNG</h2>

    <p><code>COMMAND + SHIFT + P</code> 패널을 열고 <br>
        <code>Plantuml:Export Current File Diagrams</code>를 통해서 원하는 <br>
        이미지 파일 확장자로 파일을 만들 수 있습니다.
    </p>

    <h1 id="후기">후기</h1>

    <p>처음에 web 에디터를 통해서 스크립트 작성시 <br>
        광고가 상당히 거슬렸는데 이제는 그런 불편한 점이 사라졌습니다.</p>

    <p>스크립트를 입력하면 자동으로 반영되는 점이 <br>
        시퀀스 다이어그램 작성에 많은 도움이 되었습니다.</p>

    <p>이제는 다이어그램 스크립트를 좀더 익히면 <br>
        빠르게 원하는 시퀀스 다이어그램을 만들 수 있을것 같습니다.</p>
</div>