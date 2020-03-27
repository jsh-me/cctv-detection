GOAL
-----
* 이 프로젝트는 CCTV 영상을 활용해 범인 검거를 보다 쉽게 검출할 수 있는 것을 목표로 합니다.
* 재정상 문제로 인해 값싼 CCTV를 사용하고 있는 지역은 밤 중 영상의 화질이 좋지 않기 때문에 범죄가 일어날 확률이 높습니다. 우리는 이 점을 개선하고자, Yolo를 이용하여 범인을 추적한 후 3D face로 만들어 더 쉽게 몽타주를 만들 수 있도록 개발하였습니다.

Reference
----

1. Deep3DFaceReconstruction (microsoft) github: [Microsofr Github], weights : [model]

[here]: https://github.com/microsoft/Deep3DFaceReconstruction

[model]:https://faces.dmi.unibas.ch/bfm/

2. Image Super Resolution github: [ISR]

[ISR]:https://github.com/idealo/image-super-resolution

3. Colorization github: [Colorization Github]

[Colorization Github]:https://github.com/jantic/DeOldify


Process
----

1. Yolo 사용을 위한 가상환경 설정
2. 흑백의 영상에 컬러화작업
3. 정확도가 100%인 사람의 위치를 좌표값을 저장
4. 해당 좌표값을 바탕으로 얼굴 추출
5. 추출한 얼굴의 해상도 향상
6. 3d face 제작


CCTV-No1.ipynb
----
> 프로젝트 파일은 Colab으로 실행됨

#### 0. 저장폴더 생성
- 로컬 폴더와 Google Drive 연동
- 추후에 만들어 질 파일들을 담을 폴더를 생성

#### 1. Yolo 가상환경 구축
- yolo 환경변수 세팅
- Face API 
- Yolo 출력, 업로드, 다운로드 함수 구성
- 동영상 내 사람 객체 추출 함수 구성
- Yolo 영상 및 좌표를 Google Drive 에 저장


#### 2. Log를 활용한 추출
- 동영상 내 정확도가 100% 인 사람 객체의 프레임을 txt로 저장
- 사람 객체에서 얼굴만을 따로 추출하여 face 폴더에 저장

#### 3. Face Detection and 3D Reconstruction
- Microsoft 3D Reconstruction Model weight 이용

</br>
</br>


PRESENTATION SCREENSHOTS
--------

<div>
<img width="800" src="https://user-images.githubusercontent.com/39688690/72540921-f7c74a80-38c4-11ea-97af-b88d33a8971f.png">
</div> 

<div>
<img width="800" src="https://user-images.githubusercontent.com/39688690/72540926-fa29a480-38c4-11ea-8be8-eb5b1de1bb3d.png">
</div> 

</br>
</br>

Result
------

2019년 빅데이터 청년인재 대상

</br>
</br>


