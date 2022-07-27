# Python으로 엑셀 다루기 
## 실무 상황
* DB Data를 엑셀 파일로 저장
* 기본적인 칸 정렬

## 참조 사이트
* https://book.coalastudy.com/data-crawling/week-5/stage-2 -> 코알라의 오프라인 스터디


```Python
import requests
dls = "http://www.muellerindustries.com/uploads/pdf/UW SPD0114.xls"
resp = requests.get(dls)

output = open('test.xls', 'wb')
output.write(resp.content)
output.close()
```
* https://stackoverflow.com/questions/25415405/downloading-an-excel-file-from-the-web-in-python -> stackoverflow
