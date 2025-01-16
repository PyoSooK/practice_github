# Markdown 작성법

가이드 : [https://www.markdownguide.org/](https://www.markdownguide.org/)

# 목차

### 기본 문법

- [Headings](#headings)
- [Paragraph](#paragraph)
- [Emphasis](#emphasis)
- [Highlight](#highlight)
- [Blockquotes](#blockquotes)
- [List](#list)
- [Checklists](#Checklists)
- [Code](#code)
- [Horizontal](#Horizontal)
- [Links](#links)
- [Images](#images)

# 기본 문법

# Headings

HTML : ` <h1> ~ <h6> `

Markdown : 

1. **#의 개수 (6단계)**
    
    #뒤는 항상 뛰어 써야 하며 heading 앞 뒤로 문단을 뛰어 써야 한다.
    
    ```
    # Heading 1
    
    ## Heading 2
    
    ### Heading 3
    
    #### Heading 4
    
    ##### Heading 5
    
    ###### Heading 6
    ```
    
    # Heading 1
    
    ## Heading 2
    
    ### Heading 3
    
    #### Heading 4
    
    ##### Heading 5
    
    ###### Heading 6
    

2. == 혹은 - - 사용 (상위 2단계)
    ```
    Heading 1
    =========
    
    Heading 2
    ---------
    ```
    Heading 1
    =========
    
    Heading 2
    ---------
    

# Paragraph

HTML : ` <p> `

Markdown : 

* 주의 : 문단을 작성할 때 뛰어 쓰기(스페이스, 탭)를 사용하면 안된다.

# Emphasis

1. Bold
   
   HTML : `<strong>`

   Markdown :

   (1) ** 사용
   ```
   This is **bold text**
   ```
   This is **bold text**

   (2) __ 사용
    ```
   This is __bold text__
   ```
   This is __bold text__
   

* 주의 : `This__is__bold` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 `This**is**bold`와 같이 적는 것이 좋다.
  
2. Italic

   HTML : `<em>`

   Markdown :

   (1) * 사용
   ```
   This is *Italic text*
   ```
   This is *Italic text*

   (2) _ 사용
    ```
   This is _Italic text_
   ```
   This is _Italic text_
   
* 주의 : `This_is_Italic` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 `This*is*bold`와 같이 적는 것이 좋다.

3. Bold and Italic

   HTML : `<strong><em>`

   Markdown :

   (1) *** 사용
   ```
   This is *Bold and Italic text*
   ```
   This is ***Bold and Italic text***

   (2) ___ 사용
    ```
   This is ___Bold and Italic text___
   ```
   This is ___Bold and Italic text___

   (3) __* 사용
   ```
   This is __*Bold and Italic text*__
   ```
   This is __*Bold and Italic text*__

   (4) **_ 사용
   ```
   This is **_Bold and Italic text_**
   ```
   This is **_Bold and Italic text_**
   
* 주의 : `This___is___Italic` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 `This***is***bold`와 같이 적는 것이 좋다.


# Highlight

HTML : `<mark>`

Markdown : `==` 사용

```
하이라이트 하고 싶은 부분에 ==강조== 하면 된다.
```
하이라이트 하고 싶은 부분에 <mark>강조</mark> 하면 된다.

* == 사용이 안되는 경우 `<mark>`를 사용할 수 있다.  

# Blockquotes

1. Blockquotes
   ```
   > 기호를 구문 앞에 작성하면 된다.
   ```
   > 구문 작성

2. Blockquotes with Multiple Paagraphs
   ```
   > 여러줄을 하고 싶은 경우
   >
   > 기호를 이어서 작성하면 된다.
   ```
   > 구문 작성 시작
   >
   > 구문 작성 끝
   
3. Nested Blockquotes
   ```
   >
   >> 이중 Blockquotes도 가능하다.
   ```
   > 구문 작성
   >> 이중 작성

4. Blockquotes with Other Elements
   ```
   > ## 다른 요소들을 사용할 수 있다
   >
   > - 예를 들어 강조를 사용할 수 있다
   >
   > **강조** 와 *이탤릭*
   ```
   > ### 다른 요소들을 사용할 수 있다
   >
   > - 예를 들어 강조를 사용할 수 있다
   >   
   > **강조** 와 *이탤릭*
   
# List 

1. Ordered Lists
   
   HTML : `<ol> <li>`

   Markdown :
   ```
   1. 리스트1
   2. 리스트2
   3. 리스트3
   6. 리스트6
   ```

   1. 리스트1
   2. 리스트2
   3. 리스트3
   6. 리스트6
* 숫자 순서는 상관이 없이 1번부터 순서대로 작성된다.

2. Unordered Lists
   
   HTML : `<ul> <li>`

   Markdown : 
   ```
   -, *, + 사용 (이중 사용 가능)
   
   - First
   - second
   - Third

   * First
   * Second
       * Indented

   + First
   ```
   - First
   - second
   - Third

   * First
   * Second
       * Indented
    
    + First
      
4. 리스트 안 추가 요소

   (1) Paragraphs
     ```
     * First
     * Second
       
       Paragraphs
   
     * Third
     ```
     
     * First
     * Second
       
       Paragraphs
   
     * Third
       
   (2) Blockquotes
     ```
     * First
     * Second
       
       > Blockquote
       
     * Third
     ```
     
     * First
     * Second
       
       > Blockquote
       
     * Third

   (3) Code Blocks
   
     리스트에서는 8개 혹은 2탭의 들여쓰기를 해야한다.
     ```
     1. 첫 번째 줄 
     2. 두 번째 줄
     
             <html>
              <head> <title>Test</title> </head>
             </html>

     3. 세번째 줄
     ```
     1. 첫 번째 줄 
     2. 두 번째 줄
     
             <html>
              <head> <title>Test</title> </head>
             </html>

     3. 세번째 줄
  
   (4) Images
     ```
     1. 첫 번째 줄
     2. 두 번째 줄

        ![이미지 이름](경로)
     
     3. 세 번째 줄
     ```
     1. 첫 번째 줄
     2. 두 번째 줄

        ![이미지 이름](경로)
     
     3. 세 번째 줄

   (5) List
     ```
     1. 첫 번째
     2. 두 번째
     3, 세 번째
       - 들여쓰기
       - 들여쓰기
     4. 네 번째
     ```
     1. 첫 번째
     2. 두 번째
     3, 세 번째
       - 들여쓰기
       - 들여쓰기
     4. 네 번째

# Checklists

Markdown : `- [ ]` 사용 (체크는 대괄호 안에 x 작성)

```
- [ ] 첫 번째 할 일
- [x] 두 번째 할 일
- [ ] 세 번째 할 일
```
- [ ] 첫 번째 할 일
- [x] 두 번째 할 일
- [ ] 세 번째 할 일

# Code 

HTML : `<code>`

Markdown :

1. backticks (`) 사용
   ```
   구 중간에 작성할 경우 ` 사용 `.
   여러 줄 작성할 경우 ` 세 개 사용 
   ```
   구 중간에 작성할 경우 ` 사용 `.

2. 네 칸 혹은 탭으로 들여쓰기
   ```
       <html>
        <head> </head>
       </html>
   ```

   <html>
        <head> </head>
    </html>

# Horizontal

Markdown : `***` 혹은 `---` 혹은 `____________` 사용 (사용시 앞 뒤 띄어쓰기

```
***
---
____
```

***
---
____
# Links

HTML : `<a>`

Markdown :
```
- 기본
  [Naver](https://www.naver.com)

- title 추가
  [Naver](https://www.naver.com "클릭시 네이버 홈페이지로 이동합니다")

- 링크 이름 사용 (이메일 포함)
  <https://www.naver.com>

  <123@example.com>
```

- 기본
  [Naver](https://www.naver.com)

- title 추가
  [Naver](https://naver.com "클릭시 네이버 홈페이지로 이동합니다")

- 링크 이름 사용 (이메일 포함)
  
  <https://www.naver.com>
  
  <123@example.com>


**+ 강조 사용 가능**
  ```
  **[Google](https://www.google.com)**

  This is the *[Markdown Guide](https://www.markdownguide.org)*

  See the section on ['code'](#code)
  ```
  **[Google](https://www.google.com)**

  This is the *[Markdown Guide](https://www.markdownguide.org)*

  See the section on [code](#code)

# Images

HTML : `<image>`

Markdown : Link 스타일에 !를 붙여서 사용한다. 

만약 Linking Image인 경우 image를 대괄호에 작성하고 링크를 작성한다.
```
[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
```
[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

