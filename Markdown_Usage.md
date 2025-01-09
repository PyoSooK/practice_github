# Markdown 작성법

가이드 : [https://www.markdownguide.org/](https://www.markdownguide.org/)

# 목차

### 기본 문법

- [Headings](#headings)
- [Paragraph](#paragraph)
- [Emphasis](#emphasis)
- [Blockquotes](#blockquotes)
- [List](#list)

# 기본 문법

## Headings

HTML : ``` <h1> ~ <h6> ```

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
    

## Paragraph

HTML : ``` <p> ```

Markdown : 

* 주의 : 문단을 작성할 때 뛰어 쓰기(스페이스, 탭)를 사용하면 안된다.

## Emphasis

1. Bold
   
   HTML : ```<strong>```

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
   

* 주의 : ```This__is__bold``` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 ```This**is**bold```와 같이 적는 것이 좋다.
  
2. Italic

   HTML : ```<em>```

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
   
* 주의 : ```This_is_Italic``` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 ```This*is*bold```와 같이 적는 것이 좋다.

3. Bold and Italic

   HTML : ```<strong><em>```

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
   
* 주의 : ```This___is___Italic``` 처럼 중간에 밑줄을 넣는 경우 구분이 어려울 수 있으므로 ```This***is***bold```와 같이 적는 것이 좋다.

## Blockquotes

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
   
## List 

1. Ordered Lists
   HTML : ```<ol>```
   
