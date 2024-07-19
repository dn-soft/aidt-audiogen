# [audioMerge : 오디오 합본용 코드]


&nbsp;&nbsp;


## Description for Project
1. 합쳐야되는 오디오파일들을 위한 코드입니다. 각 개별 js로 run합니다.
2. 오디오 사이 공백시간은 0.6s로 설정하였습니다.(각 스크립트에서 상수 const duration에 전역설정)
3. 진단평가 audio 파일을 다운받고 해당 경로를 성정해야합니다.(각 스크립트에서 const basePath에 전역설정)

&nbsp;&nbsp;


## Construction


&nbsp;&nbsp;


## 환경
1.  Node version ^20.10.0
   
2.  ffmpeg-static ^5.2.0<br/>
  Fmpeg의 정적 빌드(static build)를 제공하는 라이브러리.<br/>
  오디오 및 비디오를 다루는 다양한 명령줄 도구들을 포함하는 소프트웨어

3.  ffprobe-static ^3.1.0<br/>
   FFprobe의 정적 빌드를 제공하는 라이브러리.<br/>
   FFmpeg 패키지의 일부로, 미디어 파일의 형식, 코덱, 비트레이트, 해상도 등의 메타데이터를 분석하고 출력하는 도구

4.  fluent-ffmpeg ^2.1.3<br/>
   Node.js 환경에서 FFmpeg를 간편하게 사용할 수 있도록 도와주는 라이브러리.<br/>
   FFmpeg 명령을 작성하고 실행하는 것을 단순화하며, FFmpeg와 관련된 다양한 작업을 비동기적으로 처리할 수 있는 API를 제공

5.  xlsx ^0.18.5<br/>
   Node.js에서 Excel 파일(.xlsx 형식)을 읽고 쓸 수 있게 해주는 라이브러리


&nbsp;&nbsp;


## Need for Start
1. Node version v20.10.0 이상 필요

```
npm install
```


&nbsp;&nbsp;


## Terminal Commands for Quick start

1. 맞춤문항 오디오 합본 run
```
node audioMaker.js
```

2. 진단평가 오디오 합본 run
```
node audioCheckMaker.js
```


&nbsp;&nbsp;


## File Structure
사용되는 파트만 입력하였습니다.

```
aidt-audiogen
├── audios # 임시 저장 폴더
├── audioMaker.js # 맞춤문항용 audioMerge 코드
├── audioCheckMaker.js # 진단평가용 audioMerge 코드
├── getAudioList.js # 진단평가 오디오파일 리스트 추출 용
└── getImgList.js # 진단평가 이미지파일 리스트 추출 용
```
