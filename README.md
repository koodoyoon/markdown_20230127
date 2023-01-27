# markdown_20230127
마크다운 설명

### 11. 표
|번호|아이디|이름|레벨|이메일|등록일|
|:--------:|:--------|:--------|:--------:|:--------|:--------:|
|1|koodoyoon|구도윤|10|kooodoyoon@gmail.con|2023-01-27|
|2|kimhyeonseop|김현섭|7|kimhyeonseop@gmail.con|2023-01-27|
|3|cheonhamin|천하민|1|cheonhamin@gmail.con|2023-01-27|

### 10. 인라인
문단 중간에 `CODE`를 넣을 수 있습니다.(고정 폭 폰트를 표시해야 할 때 사용)\
예를 들어 `question_list = Question.objects.order_by('create_date')` 처럼

### 9. 강조
**Spring** 을 만끽하세요.\
*Spring* 을 만끽하세요.

### 8. 이미지 넣기
![파이참](https://github.com/koodoyoon/markdown_20230127/blob/main/doc/GAGOODA.png "파이참 툴팁")

### 7. 하이퍼링크
[e클래스](https://cafe.daum.net/pcwk "e클래스의 cafe입니다.")

### 6. 가로 라인
---
***
-------

### 5. 코드블럭
```
def index(request):
    ''' question 목록 '''
    question_list = Question.objects.order_by('create_date')  # order by 에 -가 붙으면 desc, 안붙으면 asc
    context = {'question_list': question_list}
    return render(request, 'pybo/question_list.html', context)
```

### 4. 목록
1. 아이템1
2. 아이템2
        아이템2-1
                아이템2-1-1
4. 아이템3

- 아이템 1
+ 아이템 2
  - 1단계 하위 아이템
    * 2단계 하위 아이템  

순서없는 목록
* 목록이름
- 목록
+ 목록

순서있는 목록
1. 목록이름
2. 목록
3. 목록 2번

### 3. 인용문
> 여기에 인용할 내용을 넣으면 됩니다.\
> 빈 줄이 없으면 자동으로 인용 상자에 포함이 됩니다.

### 2. 헤더
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5

### 1. 문단 구분을 위해 개행.
문단을 작성합니다.\
겨울이 가고 봄이 옵니다.
