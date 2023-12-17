## Main Idea
To understand what chinese users are talking about in game (popkart, tiancity).

get screen shot 1sec when user wants to.
```python
try:
    while True:
        screenshot = pyautogui.screenshot(region=(left, top, width, height))
            
        screenshot.save(file_path)
        # config letters
        # and translate..
        time.sleep(1)
except KeyboardInterrupt:
    return
```
and use `tesseract` to get letters from screen shot.

It will be translated to korean or english.