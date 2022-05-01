<h1>Matplotlib 기초</h1>

## plt.figure()
Figure인스턴스를 생성한다.   
Figure인스턴스는 이미지 전체의 영역을 확보한다.   
#### parameter
figsize: (width, height)의 튜플을 전달한다. 단위는 인치이다.   
dpi: 1인치당의 도트 수    
facecolor: 배경 색   
edgecolor: 외곽선의 색   

plt.figure() 로는 이미지 영역만 확보하므로 그래프에는 아무것도 그려지지 않는다.

## plt.figure().add_subplot()
그래프를 그리기 위해서는 subplot을 추가해야 한다.   
ex) plt.figure().add_subplot(111)   
111의 의미는 1x1의 첫 번째 원소란 뜻이다.   
335이면, 3x3에서의 다섯 번째 원소란 뜻이다.   
해당 부분에 subplot이 추가된다.   
또한, 기존 subplot에 덮어 씌운다.

## plt.subplot()
plt.subplot은 add_subplot과 동일한 파라미터를 갖는다.   
다른 점은 현재의 이미지영역에 추가하는 메소드라는 것이다.    
따라서 이전에 그려진 figure와 겹치는 경우, 이전의 figure를 지운다.   
또한, 모든 subplot들이 독립적으로 생성된다.

## plt.subplots()
fig와 Axes 혹은 Axes객체의 배열을 리턴한다.   
따라서 figure()와 add_subplot() 두 가지를 한 것과 동일한 결과를 낸다.   
물론, subplot들은 독립적으로 생성된다.   
ex) fig, axes = plt.subplots(2, 2)   
2x2 총 4개의 subplot을 생성한다.   

## Axes
Axes객체는 실제 이미지 데이터의 역할을 한다.   

