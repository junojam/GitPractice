#### Typora 파일 제작 실습/Git 사용 실습 파일 - 광주 2반 이준호
---------------------------------------------

### Typora

**1. 제목 크기 조절하기**

```
# 제목크기1
## 제목크기2
### 제목크기3
#### 제목크기4
##### 제목크기5
###### 제목크기6
```
# 제목크기1
## 제목크기2
### 제목크기3
#### 제목크기4
##### 제목크기5
###### 제목크기6
-------------------------------------------
**2. 목록 만들기**
```
+ 순서 없는 목록 1
- 순서 없는 목록 2
* 순서 없는 목록 3
1. 순서 있는 목록 1
2. 순서 있는 목록 2
```
+ 순서 없는 목록 1
-  순서 없는 목록 2
* 순서 없는 목록 3
1. 순서 있는 목록 1
2. 순서 있는 목록 2

---------------------------------
**3. 글씨 설정 변경하기**
```
*이탤릭체*
_이탤릭체_
**볼드체**
__이탤릭체__
~~취소선~~
```
*이탤릭체*
_이탤릭체_
**볼드체**
__이탤릭체__
~~취소선~~

---------------------------
**4. 언어 별 출력 화면 설정, 상자 만들기**
파이썬 print
````
```python
for i in range(10);
	print(i)
```
````

````
```
상자 만들기 예시
```
````

```python
for i in range(10);
	print(i)
```

```
상자 만들기
```

------------------------
**5. 링크 첨부하기**
```
[표시할 글자](이동할 주소) 형태로 작성합니다.
[google](https://google.com)을 눌러서 구글로 이동하세요.
```

[표시할 글자](이동할 주소) 형태로 작성합니다.
[google](https://google.com)을 눌러서 구글로 이동하세요.

--------------------------------
**6. 이미지 작성하기**
```
![대체텍스트](이미지 주소)형태로 작성합니다.
![Git로고](https://git-scm.com/images/logo@2x.png)
```
![대체텍스트](이미지 주소)형태로 작성합니다.
![Git로고](https://git-scm.com/images/logo@2x.png)

-----------------------
**7. 표 작성하기**
```
| 동물 | 종류 | 다리개수 |
| ---- | ---- | ---- |
| 사자 | 포유류 | 4개 |
| 닭 | 조류 | 2개 |
```
| 동물 | 종류   | 다리개수 |
| ---- | ------ | -------- |
| 사자 | 포유류 | 4개      |
| 닭   | 조류   | 2개      |

------------------------------------

### Git

1. commit 기록자를 등록하기
```
git config --global user.name "내 이름"
git config --global user.email "내 이메일"
git config --global -l
```

2. Git에서 Github로 넘어가려면

```
Git에서
1. Working Directory
2. Staging area
3. commits
의 구분으로 1, 2, 3 과정을 마친 후 
Github에 업로드 할 수 있다.
```

3. Git init

```
local directory를 git으로 관리하겠다고 정의하는 것
git init
```

4. Git status

```
git의 상태를 표시한다.
staging된 것이 올라간다.
untracked : git이 관리하지 않는 파일
tracked : git이 관리하는 파일
```

5. git add(staging)
```
git add a.txt
git add 폴더 이름
git add . (init된 폴더 내 안 된 것들을 전부 다 staging하기)
git status
```

6. git commit -m "first commit"
```
메시지 남기기
```

7. git log
```
git이 변화한 내역을 볼 수 있다.
```

8. 원격 저장소 등록
```
git remote add <이름> <주소>
git remote add origin https://github.com/junojam/GitPractice.git
```

9. 원격 저장소에 있는 파일을 삭제
```
git remote -v (repository 확인)
git remote rm <이름>
git remote remove <이름>
```

10. 원격 저장소 업로드
```
git push <저장소 이름><브랜치 이름>
git push origin master
```

11. git과 github를 잇는 간단 정리
```
로컬에서 자료를 업데이트 한다.
git add .
git commit -m "몇번째 commit, 변경내용은 무엇"
git push origin master
github에 업로드된 내용을 확인한다.
```