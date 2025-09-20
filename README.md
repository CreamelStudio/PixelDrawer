PixelDrawer

Unity에서 만든 간단한 픽셀 드로잉 툴입니다.
펜, 직선, 사각형, 원 모드를 지원하며, 마우스로 직접 텍스처 위에 그릴 수 있습니다. 실시간 미리보기와 PNG 저장/불러오기 기능도 포함되어 있습니다.

주요 기능
펜(Pen), 직선(Line), 사각형(Rect), 원(Circle) 모드 지원
드래그 시 실시간 미리보기 제공
색상 선택 가능: 빨강, 주황, 노랑, 초록, 파랑, 진파랑, 보라, 흰색, 검정, 회색
캔버스 초기화 가능
그림을 PNG 파일로 저장
기존 PNG 이미지를 불러오기 가능

사용 방법
Unity 씬에서 GameObject에 PixelDrawer 스크립트 추가
RawImage UI 컴포넌트를 DisplayUI 필드에 연결
필요에 따라 텍스처 크기(TextureWidth, TextureHeight) 조정
실행 후 마우스로 그림 그리기
왼쪽 클릭 + 드래그: 도형 또는 펜 그리기
버튼/함수 호출: 색상 및 그리기 모드 변경

ClearTexture(): 캔버스 초기화
SavePNG(filename): 현재 그림 저장
LoadPNG(path): 이미지 불러오기

예제 코드
pixelDrawer.SetModeLine();  // 선 그리기 모드로 변경
pixelDrawer.SetRed();       // 색상을 빨강으로 변경
pixelDrawer.ClearTexture(Color.white);  // 캔버스 초기화
pixelDrawer.SavePNG("myDrawing.png");   // 그림 저장

설치 방법
레포지토리 클론:
git clone https://github.com/yourusername/PixelDrawer.git

Unity 2021 이상에서 프로젝트 열기
GameObject에 PixelDrawer 스크립트 추가
RawImage UI 컴포넌트 연결
