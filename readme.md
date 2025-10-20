## Introduction to the G2D model
G2D(Grid based 2-Dimensional land surface flood model)는 한국건설기술연구원에서 개발된 격자 기반의 2차원 지표면 침수해석 모형이다. G2D 모형의 개발 연혁은 다음과 같다.

* G2D 모형은 2017년에 처음 개발되었다.
* 2018년에는 모의 속도와 안정성이 향상되었다.
* 2019년에는 QGIS plug-in으로 GUI가 개발되었다.
* 2020년에는 C++로 작성된 G2D 모형이 개발되었다.
* 2021년에는 NVIDIA GPU를 이용한 가속기법이 개발되었다.

G2D 모형은 한국건설기술연구원에서 지속적으로 개발되고 있다.  
<br/>  

## G2D GUI  
* QGIS plug-in GUI인 QG2D를 이용할 수 있다.  
  (https://github.com/floodmodel/Plugin_repository_QGIS3.10/tree/main/QG2D)
* QG2D 설치 및 실행 방법은 QG2D tutorial을 참고한다.
  (https://github.com/floodmodel/G2D/blob/master/DownloadStableVersion/QG2D_tutorial.pdf)  
<br/>  

## Download
### Latest version
* G2D model  
  G2D 모형 실행 파일(.exe), sample data, manual, source code  
  https://github.com/floodmodel/G2D/tree/master/DownloadStableVersion 에서 다운로드

### QG2D
- G2D 모형의 QGIS plugin GUI  
  https://github.com/floodmodel/Plugin_repository_QGIS3.10/tree/main/QG2D 에서 다운로드  
- QG2D 설치 및 사용 방법
  https://github.com/floodmodel/G2D/blob/master/DownloadStableVersion/QG2D_tutorial.pdf

### GPU 관련 사항 
 * G2D v.2021 부터 CUDA tool kit 11.2 환경에서 개발됨.
 * CUDA 11은 NVIDIA Driver version으로 452.39 이상을 요구(RTX Desktop Manager는 생략 가능) (CUDA Toolkit은 불필요)
 * NVIDIA 그래픽 카드를 사용하지 않는 경우 혹은 UsingGPU 옵션을 선택하지 않는 경우에도 cudart64_110.dll 파일이 필요하며, cudart64_110.dll 파일이 Windows path에 설정된 폴더 혹은 G2D.exe 파일과 같은 폴더에 있어야 함.


### vcomp140.dll 관련 사항
* Windows path로 설정된 위치에 VCOMP140.DLL가 필요하며, 구체적으로는 아래를 참고
  * 만일 OS가 Windows 11이면 문제 없음   
  * 만일 OS가 Windows 10이면 아래의 방법 중 하나를 이용해서 VCOMP140.DLL 파일을 설치 할 수 있음
    +	Visual Studio 2015 혹은 (VCOMP140.DLL 파일이 포함된) 그 이상의 버전 설치  
    +	Microsoft Visual C++ 2015 Redistributable 혹은 (VCOMP140.DLL 파일이 포함된) 그 이상의 버전 설치  
    +	NVIDIA driver 536.67 혹은 (VCOMP140.DLL 파일이 포함된) 그 이상의 버전을 default(RTX Desktop Manager 설치 포함) 설정으로 설치
    +	QGIS 3.10.14 혹은 (VCOMP140.DLL 파일이 포함된) 그 이상의 버전을 설치하고 "C:\Program Files\QGIS 3.10\bin\"를 Windows path에 추가. QGIS 폴더명은 QGIS 버전에 따라서 변경될 수 있음.  
<br/>  

## YouTube video clips
- Data processing tools : [**[Link]**](https://www.youtube.com/watch?v=iC3Qa9iwcus&t=62s)  
- The G2D model : [**[Link]**](https://www.youtube.com/watch?v=lnXc0Z8PRyY)  
- Introduction to the GRM and G2D model (ETRI Open Source Tech Day 2021) : [**[Link]**](https://www.youtube.com/watch?v=OFRqzLPlD2Q)   

