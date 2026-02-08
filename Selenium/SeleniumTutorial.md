## Selenium Start (Python 기준)
## 사전 조건
- Chrome 브라우저가 설치
- python 설치 (python3 추천)

### 1. 설치

pip install selenium webdriver-manager

### 2. 예제 코드

```python
from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager

driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))
driver.get("https://example.com")

print(driver.title)
print(driver.find_element("tag name", "h1").text)
driver.quit()
```

### 3. 실행
```
python example.py
```
