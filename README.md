# MS_learn_trophy
Microsoft Learn 프로필 링크를 url에 넣으면 url대상자가 수료한 과정을 출력.

**사용설명서: Microsoft Learn 챌린지 완료 여부 확인 스크립트**

이 사용설명서는 Python Selenium을 사용하여 Microsoft Learn 프로필에서 특정 챌린지의 완료 여부를 확인하는 스크립트에 대한 설명을 제공합니다.

**1. 필수 요구사항**
- Python 3.x 버전 이상
- Selenium 패키지 설치
- Chrome 브라우저
- ChromeDriver 설치 (https://chromedriver.chromium.org/downloads 에서 Chrome 버전에 맞는 드라이버 다운로드)

**2. 스크립트 설치 및 설정**
- Python 환경에서 위의 코드를 사용하려는 디렉토리에 저장합니다.
- `webdriver_service` 변수에서 ChromeDriver 경로를 올바른 경로로 수정합니다. (예: `webdriver_service = Service('./chromedriver_mac64/chromedriver.exe')`)
- 필요에 따라 다른 옵션을 설정할 수 있습니다. (예: `options.add_argument('--headless')`는 브라우저를 표시하지 않고 실행하는 옵션입니다.)

**3. 스크립트 실행**
- 터미널 또는 명령 프롬프트에서 스크립트를 실행합니다.
- 실행 중에는 Microsoft Learn 프로필의 링크를 입력하라는 메시지가 표시됩니다. Microsoft Learn 프로필 페이지의 URL을 입력합니다.
- 다음으로, 완료 여부를 확인하려는 챌린지 코드를 입력하라는 메시지가 표시됩니다. 확인하려는 챌린지의 코드를 입력합니다. (예: `AZ-900`)
- 스크립트는 입력한 프로필에서 해당 챌린지의 필수 배지가 있는지 확인하고 결과를 표시합니다.

**4. 결과 해석**
- 스크립트는 해당 챌린지의 필수 배지가 모두 있는 경우 "완료 /ok"를 출력합니다.
- 필수 배지 중 하나라도 없는 경우 "NO"를 출력합니다.

**5. 스크립트 종료**
- 스크립트 실행이 완료되면 브라우저가 종료됩니다.

**참고 사항**
- 스크립트는 Microsoft Learn 프로필의 배지 제목이 코드에 기재된 것과 동일하다고 가정합니다. Microsoft Learn 플랫폼에서 배지 제목이 변경된 경우 코드를 업데이트해야 합니다.
- 스크립트의 실행 결과는 콘솔에 표시됩니다. 필요에 따라 코드를 수정하여 결과를 파일에 저장하거나 다른 방식으로 처리할 수 있습니다.
