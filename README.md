# ZoomBot

```python
from selenium import webdriver
import datetime
from datetime import date
import time


PATH = "C:\\Users\\emu4y\\Desktop\\chromedriver.exe"
driver = webdriver.Chrome(PATH)

def open_up_zoom():
    now = datetime.datetime.now()
    endOfSchool = now.replace(hour = 15, minute = 0, second = 0, microsecond = 0)
    print(now)
    if date.today().weekday() == 0 or date.today().weekday() == 3:
        fPer = now.replace(hour = 8, minute = 30, second = 0, microsecond = 0)
        tPer = now.replace(hour = 10, minute = 10, second = 0, microsecond = 0)
        fivePer = now.replace(hour = 12, minute = 20, second = 0, microsecond = 0)
        if fPer <= now <= fPer.replace(hour = 8, minute = 30, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/94055272968?pwd=SnBteGxyQWtTOUtDL09lTWRTSGJMUT09")
        if tPer <= now <= tPer.replace(hour = 10, minute = 10, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/91028268141?pwd=ZmJJN3ZxNzdzNUdGNHZMc0JYZXZKdz09")
        if fivePer <= now <= fivePer.replace(hour = 12, minute = 20, second = 10, microsecond = 0):
            driver.get("https://us02web.zoom.us/j/88557268811?pwd=ZEY5L2c4dmRBTjQwajkzYkhGRjJDZz09")

    if date.today().weekday() == 2:
        fPer = now.replace(hour = 8, minute = 30, second = 0, microsecond = 0)
        tPer = now.replace(hour = 10, minute = 10, second = 0, microsecond = 0)
        fivePer = now.replace(hour = 12, minute = 20, second = 0, microsecond = 0)
        sPer = now.replace(hour = 9, minute = 20, second = 0, microsecond = 0)
        foPer = now.replace(hour = 11, minute = 0, second = 0, microsecond = 0)
        sixPer = now.replace(hour = 13, minute = 10, second = 0, microsecond = 0)
        if fPer <= now <= fPer.replace(hour = 8, minute = 30, second = 10, microsecond = 0):
            driver.get("https://tinyurl.com/busownper2")
        if sPer <= now <= sPer.replace(hour = 9, minute = 20, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/93696944656?pwd=R0ZncXVsVm0wQlJReDZjTmE3SXN3QT09")
        if tPer <= now <= tPer.replace(hour = 10, minute = 10, second = 10, microsecond = 0):
            driver.get("https://us02web.zoom.us/j/86319878388?pwd=Tyswdmx3R2kwNkEvY0lSazNlS2tiZz09")   
        if foPer <= now <= foPer.replace(hour = 11, minute = 0, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/94055272968?pwd=SnBteGxyQWtTOUtDL09lTWRTSGJMUT09")
        if fivePer <= now <= fivePer.replace(hour = 12, minute = 20, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/91028268141?pwd=ZmJJN3ZxNzdzNUdGNHZMc0JYZXZKdz09")
        if sixPer <= now <= sixPer.replace(hour = 13, minute = 10, second = 10, microsecond = 0):
            driver.get("https://us02web.zoom.us/j/88557268811?pwd=ZEY5L2c4dmRBTjQwajkzYkhGRjJDZz09")


    if date.today().weekday() == 1 or date.today().weekday() == 4:
        sPer = now.replace(hour = 8, minute = 30, second = 0, microsecond = 0)
        foPer = now.replace(hour = 10, minute = 10, second = 0, microsecond = 0)
        sixPer = now.replace(hour = 12, minute = 20, second = 0, microsecond = 0)
        if sPer <= now <= sPer.replace(hour = 8, minute = 30, second = 10, microsecond = 0):
            driver.get("https://tinyurl.com/busownper2")
        if foPer <= now <= foPer.replace(hour = 10, minute = 10, second = 10, microsecond = 0):
            driver.get("https://zoom.us/j/94564395111?pwd=cU5VVURVaGxtR0xtYUwrZTUwaEt5QT09")
        if sixPer <= now <= sixPer.replace(hour = 12, minute = 20, second = 10, microsecond = 0):
            driver.get("https://us02web.zoom.us/j/86319878388?pwd=Tyswdmx3R2kwNkEvY0lSazNlS2tiZz09")   

try: 
    while True:
        open_up_zoom()
        time.sleep(10)
except KeyboardInterrupt:
    print("gg")
```
