# python_programming
##python homework

this repository 는 파이선 프로그래밍 수업 숙제를 위한 저장소 입니다.

### [HomeWork 02주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw1/Types(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
### [HomeWork 02주차-02](https://github.com/lim-ilyong/python_programming/blob/main/hw1/Strings(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)

### [HomeWork 03주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw2/Tuples(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
### [HomeWork 03주차-02](https://github.com/lim-ilyong/python_programming/blob/main/hw2/Lists(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * Tuple vs. List //  * Tuple : 수정 불가, 빠름   * List : 수정 가능(강력함), 무거움
  * Copy vs. Clone // * 주소 복사  * Clone 방법 list명[:]
  * extend vs. append // extend 확장, append 엘레멘트 1개로 추가    
### [HomeWork 03주차-03](https://github.com/lim-ilyong/python_programming/blob/main/hw2/Dictionaries(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * dictionary는 {}를 사용하여 key:value,  key:value, … 로 정의			
  * dict.keys()			
  * dict.values()			
  * 추가 : dict(key:value) 추가 :마지막 삽입			
  * del(dict['Thriller'])  : 삭제는 del함수 사용			
  * Thriller' in release_year_dict : key값이 있는지 체크			

### [HomeWork 04주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw3/Conditions(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * if 조건 :
  * elsif 조건 :
  * else :
  * 중요 : 과 indentation 중요

### [HomeWork 05주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw4/Loops(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * for i in range(-5,6) : 
  * while ( ) :
  * 중요 문법 : for 또는 while 끝에 :(콜론) 주의


### [HomeWork 06주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw5/Functions(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * function 들여쓰기 주의
  * 전역변수, 지역변수

### [HomeWork 06주차-02](https://github.com/lim-ilyong/python_programming/blob/main/hw5/Classes(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * class , 생성자, method, 속성


### [HomeWork 07주차-01](https://github.com/lim-ilyong/python_programming/blob/main/hw6/ReadFile(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * [mount]
    from google.colab import drive
    drive.mount('/content/gdrive')
  * [read]
    example1 = "/content/gdrive/My Drive/Colab Notebooks/Example1.txt"
    with open(example1, "r") as file1:
         for line in file1:
             print(file1.readline())

### [HomeWork 07주차-02](https://github.com/lim-ilyong/python_programming/blob/main/hw6/WriteFile(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
   * [mount]
     from goole.colab import drive
     drive.mount('/content/gdrive')
   * [write]
     example2 = "/content/gdrive/My Drive/Colab Notebooks/Example2.txt"
     Lines = ["This is line A\n", "This is line B\n", "This is line C\n"]
     with opne(example2, "w") as file2:
         for line in Lines:
             file2.write(line)


### [HomeWork 07주차-03](https://github.com/lim-ilyong/python_programming/blob/main/hw6/LoadData(Pandas)(%ED%95%99%EC%83%9D%EC%9A%A9).ipynb)
  * [mount]
    from google.colab import drive
      drive.mount('/content/gdrive')

    csv_path = '/content/gdrive/My Drive/Colab Notebooks/TopSellingAlbums.csv'
    df = pd.read_csv(csv_path)
    df1.head()
    df.tail()
    
   y = df[['Artist','Length','Genre']]  
   df.iloc[0, 0] #첫번째 행, 첫번째 열 
   df.loc[0, 'Artist']

   df.iloc[0:2, 0:3] #row, column sequence 

   df.loc[0:2, 'Artist':'Released'] #iloc, loc의 차이점이 있음...

   # iterating over rows using iterrows() function 

   for i, j in df.iterrows():
       print(i, j)
       print()


    다른 예.
    filter2 = df["Claimed Sales (millions)"]>40

