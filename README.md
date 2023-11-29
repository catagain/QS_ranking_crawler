# QS Ranking Crawler
## Sustainability:
To retrieve information from the webpage (https://www.topuniversities.com/university-rankings/sustainability-rankings/2023), locate the ID as shown in the image below. Replace the ID part in the code where the webpage URL is.

```python
school_page = requests.request('Get', 'https://www.topuniversities.com/sites/default/files/qs-rankings-data/en/ID_of_year.txt?rmvlzx')
```
![image](https://github.com/catagain/QS_ranking_crawler/assets/35026988/a2247b75-7e30-4348-a2bd-9de8d7029668)

## World Ranking:
Similar to the Sustainability section, find the ID and replace it in the URL used in the requests call.

## Employment Ranking Crawler:
For data before 2022, there might have been changes in field names. Use the function call directly with the year parameter.

## Subjects:
For a specific year, go to the def QS_crawling(subject, page): function and modify the URL with the desired year. Specifically, this line needs to be adjusted:

```python
browser.get('https://www.topuniversities.com/university-rankings/university-subject-rankings/2023/' + subject + '?&page=' + str(page) + '&tab=indicators')
```
When calling the function, refer to the QS website (https://www.topuniversities.com/subject-rankings) to choose a subject of interest and use its name to crawl.

For example:

```python
get_subject('philosophy', 0)
```

# QS_ranking_crawler

## Sustanibility：
要去網頁（https://www.topuniversities.com/university-rankings/sustainability-rankings/2023）找到 id（如下圖），把程式碼中 request 的網址 ID 部分替換掉
```python
school_page = requests.request('Get', 'https://www.topuniversities.com/sites/default/files/qs-rankings-data/en/ID_of_year.txt?rmvlzx')
```
![image](https://github.com/catagain/QS_ranking_crawler/assets/35026988/a2247b75-7e30-4348-a2bd-9de8d7029668)



## World Ranking：

同上，找到 id 後，替換 request 的網址中的 id 

## 就業力排名爬蟲：

2022 年以前的東西，現在可能已經有不少欄位有改動，呼叫都是直接用年分 call function。

## Subjects：
針對特定年分，要去 def QS_crawling(subject, page): 中，修改網址年份。
具體是這一行
```python
browser.get('https://www.topuniversities.com/university-rankings/university-subject-rankings/2023/' + subject + '?&page=' + str(page) + '&tab=indicators')
```
呼叫 function 時，可以參考 QS 網站（https://www.topuniversities.com/subject-rankings ），選其中有興趣的學科，用其名子來爬。
e.g. 
```python
get_subject('philosophy', 0)
```


