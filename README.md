# Detection of CCTV Using Deep Learning

* 이 프로젝트는 CCTV 영상을 활용해 범인 검거를 보다 쉽게 검출할 수 있는 것을 목표로 합니다.
* 재정상 문제로 인해 값싼 CCTV를 사용하고 있는 지역은 밤 중 영상의 화질이 좋지 않기 때문에 범죄가 일어날 확률이 높습니다. 
* 우리는 이 점을 개선하고자, Yolo를 이용하여 범인을 추적하고, 얼굴을 뽑아내 3D face로 만들어 더 쉽게 몽타주를 만들 수 있도록 개발하였습니다.

Reference
----

1. Deep3DFaceReconstruction (microsoft) github: [here], weights : [model]

[here]: https://github.com/microsoft/Deep3DFaceReconstruction

[model]:https://faces.dmi.unibas.ch/bfm/

2. Image Super Resolution github: [here!]

[here!]:https://github.com/idealo/image-super-resolution

3. Colorzization github: [here!!]

[here!!]:https://github.com/jantic/DeOldify


Process
----

1. Yolo 사용을 위한 가상환경 설정.
2. 흑백의 영상에 컬러화작업
3. 정확도가 100%인 사람의 위치를 좌표값으로 return.
4. 해당 좌표값을 가져오면 전신사진이 저장이 되는데, 그 중 얼굴을 따로 추출. 
5. 추출한 얼굴의 해상도를 올림.
6. 3d face 제작

PPT SCREENSHOTS
--------
<div>
<img width="800" src="https://user-images.githubusercontent.com/39688690/72540921-f7c74a80-38c4-11ea-97af-b88d33a8971f.png">
</div> 

<div>
<img width="800" src="https://user-images.githubusercontent.com/39688690/72540926-fa29a480-38c4-11ea-8be8-eb5b1de1bb3d.png">
</div> 

<div>
<img width="800" src="https://user-images.githubusercontent.com/39688690/72540932-fbf36800-38c4-11ea-9e75-2e1abe3d4143.png">
</div> 


Result
------

2019년 빅데이터 청년인재 대상 수상





sorry :-( The output result cannot be displayed due to the right of likeness.


