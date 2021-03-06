
Colab에 대해서 
=============

## 1. 구글 코랩이란?

+ 구글 코랩은 구글이 제공하는 주피터 노트북을 말합니다.    
+ 주피터 노트북이란 프로그램 코드를 브라우저에서 실행해주는 대화식 환경입니다. 코랩은 브라우저를 통해 구글 클라우드의 가상 서버를 사용합니다. 즉, 구글이 제공하는 컴퓨터로 실습할 수 있다는 것입니다. 코랩은 구글에서 교육, 과학연구를 목적으로 개발한 도구이며 2017년에 무료로 공개되었습니다.   
+ 코랩에서 파이썬 코드를 실행하거나 텍스트를 저장할 수 있고 그래프를 그릴 수도 있습니다. 사용자가 웹브라우저를 통하여 코랩에 코드를 짜서 실행하면, 그 내용이 구글 클라우드에게 전달되어 코드 실행을 시킨 후 실행결과를 사용자에게 다시 건네줍니다.   
+ 이러한 기능들은 모두 구글에서 제공하며 구글과 연관되어 있기 때문에 구글 계정이 반드시 필요합니다.   
+ 주피터 노트북에는 코드 셀과 텍스트 셀이 있습니다. 텍스트 셀은 말 그대로 텍스트를 입력하여 글을 쓸 수 있습니다.    

  + 텍스트 셀 추가하기
    
   <img src="https://user-images.githubusercontent.com/50646904/97397582-f4b9ba00-192c-11eb-8236-d5b632834f58.PNG" width="500px" height="300px" title="px(픽셀) 크기 설정" alt="1"></img><br/> 

  + 텍스트 셀 수정하기
  
   <img src="https://user-images.githubusercontent.com/50646904/97397586-f5525080-192c-11eb-88c3-0587b16dc244.PNG" width="500px" height="300px" title="px(픽셀) 크기 설정" alt="2"></img>   
+ 위의 사진에서 마우스로 셀을 더블 클릭하거나 셀을 선택한 상태에서 엔터를 누르면 간편하게 텍스트 셀의 내용을 수정할 수 있습니다. 코랩은 마크다운을 사용하여 특수기호와 문자를 표현합니다.
   
  + 코드 셀 작성하기
  ![코드](https://user-images.githubusercontent.com/50646904/97397587-f5eae700-192c-11eb-8f2f-d3d414ce37fc.PNG)
+ 코드 셀을 추가한 후 작성하고자 하는 코드를 셀 안에 적은 후, 왼쪽의 재생 버튼이나 컨트롤과 엔터를 함께 누르면 실행이 됩니다. 새로운 코드 셀을 추가하는 방법은 왼쪽 위의 +코드를 클릭하거나 쉬프트와 엔터를 동시에 입력하면 간편하게 코드 셀이 추가됩니다.   
+ 코드를 실행시키기 전 런타임-> 런타임 유형 변경에 들어가 하드웨어 가속기가 알맞게 설정되었는지 확인해야 합니다. TPU는 데이터 분석 및 딥러닝용 하드웨어 이며, GPU는 그래픽 프로세서 유저 인터페이스를 의미합니다.  
+ 이렇게 작성한 노트북을 저장하려면 어떻게 해야하는가? 파일-> 구글 드라이브에 저장을 누르면 지금까지의 작업이 구글 드라이브에 저장됩니다. 저장된 노트북은 파일->드라이브에서 찾기를 선택하면 노트북이 저장된 위치를 새 탭으로 보여줍니다. 이렇게 저장된 파일은 내 드라이브에 저장되어있기 때문에 언제든지 접근하여 사용할 수 있습니다. 또한, 새로만들기를 클릭하여 폴더를 만든 후 그 폴더 안에 노트북을 저장할 수도 있고, 코랩 자체에서 파일-> 노트북 열기를 하면 이전에 사용했던 노트북이나 구글 드라이브에 있는 노트북을 손쉽게 열 수 있습니다. 

---------------------
## 2. 구글 코랩은 어떤 기술 스택을 모은 것인가?
+ 구글 코랩은 코랩+ 구글드라이브+ 도커+ 리눅스 +구글클라우드의 기술 스택으로 이루어져있습니다.   
코랩은 구글 드라이브와 구글 클라우드를 이용하여 코드의 작성과 실행의 전반적인 과정을 수행합니다. 도커는 컨테이너 기반의 오픈소스 가상화 플랫폼인데, 프로그램과 실행환경을 컨테이너로 추상화하고 동일한 인터페이스를 제공하여 프로그램의 배포 및 관리를 단순하게 해줍니다. GitHub로 코드를 보내거나 구글 클라우드로 코드를 전송하여 실행하는 과정에서도 도커가 사용됩니다. 2014년 발표에 따르면 구글은 모든 서비스들이 컨테이너로 동작하고 매주 20억 개의 컨테이너를 구동한다고 합니다. 
---------------------
## 3. 구글 코랩의 장점은?
+ 환경설정 및 구동 준비가 빠른 시간 내에 끝납니다.
+ 딥러닝 분야는 연산 비용이 높아 컴퓨터의 성능이 중요한데, 코랩을 사용하면 구글 클라우드의 가상 서버를 마음껏 활용할 수 있습니다. 
+ 딥러닝 개발을 위한 라이브러리를 이미 포함하고 있고, GitHub 등과의 연동을 통해 소스를 업로드하고 다운로드할 수 있는 개발 환경을 제공합니다.
+ 보통 개인PC보다 성능이 좋으며 클라우드 기반이기 때문에 여러 명이 동시에 수정할 수 있고, 인터넷 브라우저에 접속할 수만 있다면 코드 수정이 가능합니다. 
+ 오류가 발생했을 때 **SEARCH STACK OVERFLOW** 버튼을 클릭하면 자동으로 스택오버플로우 사이트의 검색 결과가 나타납니다. 
------------------------
## 4. 구글 코랩의 단점은?
+ 최대 세션 유지시간이 12시간입니다. 12시간이 지나면 세션이 끊기기 때문에 작업중이던 데이터를 잃지 않도록 상시 저장해야 합니다. 
+ 딥러닝을 학습시킬 데이터는 구글 드라이브에 저장해 놓되, 개인이 사용할 수 있는 최대 용량은 15G이기 때문에 많은 양의 데이터를 학습시켜야 하는 상황이라면 일정 비용을 지불하여 30G이상의 용량을 사용하도록 해야합니다. 
+ 금융권과 같은 망분리 보안 이슈로 법적으로 클라우드에 데이터를 올릴 수 없는 경우는 활용할 수 없습니다. 
------------------------
## 5. 구글 코랩의 접속방법은?
+ 크롬 부라우저에 접속하여 구글 드라이브에 들어가서 로그인을 하면 개인용 구글드라이브에 이동할 수 있습니다. 코랩이 이미 설치되어 있는 경우에는 새로만들기->더보기->Colab 의 순서로 진행하면 코랩에 접속할 수 있고, 코랩이 설치되어있지 않은 경우에는 더보기-> 연결할 앱 더보기에서 돋보기버튼을 클릭하여 **Colaboratory** 를 검색해서 설치하면 사용할 수 있습니다. 
-------------------------
## 6. 작성소감
구글 드라이브는 이따금씩 사용해본 적이 있는데, 코랩이라는 기능이 있는 지는 전혀 몰랐습니다. 파이썬을 설치하지 않고도구글 클라우드 서버를 연결하여  파이썬의 기능을 사용할 수 있는 점이 혁신적으로 느껴졌고, 사용법만 잘 익힌다면 유용하게 쓸 수 있을 것 같습니다.    
특히 구글 드라이브에 저장하여 브라우저에 접속만 가능하다면 어떤 컴퓨터에서든 코드를 읽고 수정하고 실행할 수 있다는 점이 굉장히 편리해보였습니다. 자취방에서 지내다 보니 본가에 종종 가고는 하는데, 노트북의 무게가 상당하여 들고 다니기 힘들었습니다. 하지만 본가에 있는 컴퓨터는 성능이 좋지 못해서 힘들더라도 노트북을 항상 가지고 본가에 가고는 했는데 이제는 코랩을 사용하여 이러한 문제를 해결할 수 있을 것 같습니다.    
그리고 구글 클라우드에 이미 tensorflow 등 딥러닝에 필요한 기본 패키지들이 깔려있어 코랩으로 딥러닝을 하기에 용이하다고 하니 딥러닝을 어서 학습해보고 싶은 마음이 듭니다.    
처음 시작할 때는 인공지능, 딥러닝 이런 분야가 멀게만 느껴졌는데 지금은 굉장히 가까이에 있는 것 처럼 느껴집니다. 열심히 공부하여 배움이 헛되지 않도록, 배운 것들을 잘 활용하여 자율주행 자동차 같이 세상을 한층 더 편리하게 만들어 주는 프로그램을 개발하고 싶습니다. 
