## Main Idea
To understand what chinese users are talking about in game (popkart, tiancity).\

get screen shot 1sec when user wants to.
```python
def getScreenShot():
    try:
        while True:
            # 화면 좌표에 해당하는 부분의 스크린샷 찍기
            screenshot = pyautogui.screenshot(region=(left, top, width, height))
            
            # 스크린샷 저장
            screenshot.save(file_path)
            
            # 일정 시간 대기
            time.sleep(1)
    except KeyboardInterrupt:
        return
```
and use `tesseract` to get letters from screen shot.

It will be translated to korean or english.