### Study_Python
Hello, This is Beginner      

> I'm learning here        
> : https://github.com/bnv20    
<br>


파이썬공부  [1주차_내용]
1) 파이썬 기초
2) 자료형 - 리스트, 튜플, 딕셔너리, 집합
3) 프로그램 구조 쌓기 - if, while, for
4) 함수
5) 모듈, 패키지, 라이브러리 간단정리.

\
파이썬공부  [2주차_내용]
1) 예외처리 try, else, except, finally
2) 클래스 - 객체지향언어     
3) 프로그램에 대한 공부

\
파이썬공부  [3주차_내용_1]
1) . ^ $ * + ? {} [] \ | () 메타문자     
2) 정규표현식 re.match, re.search, re.findall, re.finditer, re.split(), re.sub()    
3) web_crawling_기초 
4) import requests -> requests.get(URL), .text,/bs4, soup = / re.sub('<.+?>','',text)
5) import urllib -> urllib.request.Request(URL), urllib.request.urlopen(URL), .read(), .decode('utf-8')
6) #웹 이미지 저장 urllib.request.urlretrieve(img_src, 저장파일name)
7) BeautifulSoup -> HTML 태그들을 parser : 'html.parser' =='lxml'
8) title = soup.find(id='title') => find(속성 ='값')
9) html tag 정리 
10) find(), find_all() / select_one(), select() _CSS 선택자를 활용, class는 .으로 id는 #로 표시
11) selenium 모듈 web driver 별도설치!!후 이용, 웹 제어 driver = webdriver.Chrome(드라이버위치;path)
12) driver.get(url), driver.close(), .click() , .send_keys('텍스트 입력'), .send_keys(Keys.RETURN)
13) find_element(s)_by ~~
14) #자바스크립트 실행 driver.execute_script()
15) page_source 가져오기, bs = BeautifulSoup(driver.page_source, 'html.parser')
16) #web browser 화면캡쳐, driver.get_screenshot_as_file('dataset/naver.png';경로 및 파일이름)
17) 탭이동, driver.switch_to_window(driver.window_handles[-1])

\
파이썬공부  [3주차_내용_2]
1) pandas_데이터형식
2) 데이터프레임 , index > 행, columns > 열  
3) 2차원 리스트 -> 데이터프레임으로 변환
4) pd.concat, df.drop, df.query('index==0'), df.loc[], df.ilon[], df[[]]
5) df.set_index, df.reset_index(), df.add(), df.reindex(), df.sort_index(), df.sort_values()
6) 행추가, 열추가, df.transpose()
7) pandas_입출력, df.to_csv(), pd.read_csv(index_col=0), df.describe()
8) json 파일 df.to_json(), 바이너리파일 df.to_pickle(), 엑셀파일 df.to_excel()
9) pandas_연산, df.add(df, fill_value = 빈 값 채우기), sub, mul, div
10) 데이터프레임에서 시리즈 더하고 빼고 계산 df.rdiv(), rmul, radd, rsub

\
파이썬공부  [4주차_내용_1]
1) 판다스 옵션중에 out[ ]에 보여지는 행과 열 수 조절하는 방법
2) 데이터세트에 파악 .info(), .columns, .index, .describe(), .corr(), .value_counts(), .unique()
3) from collections import Counter, Counter(리스트)
4) .round()  #딕셔너리로 컬럼 각각 설정 가능
5) Null 값, df.fillna(), df.dropna(), df[].isnull().sum()
6) df.astype(바꿀타입), df.reindex(원하는 행,열, 행과열)
7) pd.concat( ), pd.merge( ), df.join(df2, isuffix='',rsuffix=''), df.groupby( ), df.apply( )
8) 범주화
9) 결측치 처리 df.fillna(특정값), df.fillna(method='ffill'), df.fillna(method='bfill'), df.fillna(df.mean())
10) df.drop_duplicates(), .replace(), rename() 
11) 인코딩 - LableEncoder/OneHotEncoder, 스케일링 - 정규화/표준화,로그변환

\
파이썬공부  [4주차_내용_2]
1) 크롤링 응용
2) #html 자식들 출력, #자손까지, #부모노드 구하기
3) 정규표현식과 bs4 짬뽕
4) 로그인 후 자료 가져오기
5) driver.page_source 가져와서 BeautifulSoup이용
6) driver.execute_script('document.getElementById("id").value="{id}"; document.getElementById("pw").value="{pw}"'.format(id='ID',pw='PW'))
7) 화면 가장 아래로 스크롤 내리기; driver.execute_script('window.scrollTo(0,document.body.scrollHeight)')
8) headless chrome, options = webdriver.ChromeOptions() + options.headless = True
