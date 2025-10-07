
viewer_starter 사용법 (B안: Three.js + 설정 파일 기반)

1) 압축을 풀고, VS Code에서 폴더를 엽니다.
2) VS Code 확장 'Live Server'를 설치한 뒤 index.html을 'Open with Live Server'로 실행하세요.
3) 브라우저 주소창에 아래처럼 입력:
   http://127.0.0.1:5500/index.html?cfg=projects/demo/config.json

4) projects/demo/assets/ 폴더에 본인의 GLB(예: sample.glb)를 넣습니다.
   (config.json의 "asset": "assets/sample.glb" 경로는 config.json 기준 상대경로입니다.)

5) 측정/단면/스냅샷/텍스처 토글/뷰 전환을 바로 테스트할 수 있습니다.

팁:
- glTF(.gltf)도 로드 가능하지만, .bin/텍스처 파일이 config.json에서 지정된 위치 기준으로
  상대 경로가 맞아야 합니다. GLB 단일 파일을 우선 추천합니다.
- 단면 축은 config.json의 ui.sectionAxis 값을 x|y|z로 바꿔 조절할 수 있습니다.
- 단위 변환은 units.world_to_unit 값을 조절하세요. (예: world_to_unit=0.001 이면 1 world unit=0.001 mm)
