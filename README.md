# 점심 메뉴 추천 웹 애플리케이션

이 웹 애플리케이션은 사용자가 입력한 텍스트를 바탕으로 두 가지 AI 모델을 통해 점심 메뉴를 추천받을 수 있는 시스템입니다. 입력한 텍스트에 대해 추천된 메뉴를 확인하고, 필요 시 삭제할 수 있습니다.

## 기능
- **모델 선택**: 두 가지 AI 모델 (`gemini-1.5-flash`, `deepseek-r1`) 중 하나를 선택하여 점심 메뉴를 추천받습니다.
- **데이터 저장**: 로컬 스토리지를 사용하여 사용자가 입력한 텍스트와 AI의 답변을 저장하고, 페이지를 새로 고침해도 데이터를 유지합니다.
- **삭제 기능**: 추천 목록에서 개별 항목을 삭제할 수 있습니다.
- **리셋 버튼**: "저장된 데이터 리셋" 버튼을 클릭하여 저장된 데이터를 삭제할 수 있습니다.

## 사용 방법
1. **모델 선택**: 드롭다운 메뉴에서 원하는 모델을 선택합니다.
2. **텍스트 입력**: 점심 메뉴 추천을 위한 텍스트를 입력합니다.
3. **등록**: '등록' 버튼을 클릭하면 해당 텍스트를 기반으로 모델이 점심 메뉴를 추천합니다.
4. **삭제**: 기존에 저장된 항목 옆의 "삭제" 버튼을 클릭하여 데이터를 삭제할 수 있습니다.
5. **리셋**: "저장된 데이터 리셋" 버튼을 클릭하면 로컬 스토리지에 저장된 모든 데이터가 삭제됩니다.

## 기술 스택
- **HTML**: 웹 페이지 구조
- **CSS**: 기본 스타일링
- **JavaScript**: 동적 데이터 처리, 로컬 스토리지 사용, API 호출
- **Proxy**: 데이터 변화 추적 및 화면 갱신
- **Fetch API**: AI 모델과의 통신을 위한 API 요청

## API
- **Gemini 모델 (1.5-Flash)**: `https://spotted-famous-seaplane.glitch.me/1`
- **DeepSeek 모델 (R1)**: `https://spotted-famous-seaplane.glitch.me/2`

## 설치 방법
1. 이 저장소를 클론합니다.
   ```bash
   git clone <repository-url>
