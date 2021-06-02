👻TIL-10👻

# form 태그
: 웹 서버에 정보를 제출하기 위한 양식 범위를 정의한다.

![image](https://user-images.githubusercontent.com/67450413/120430755-75083800-c3b2-11eb-8e58-ad001f3342ee.png)
- action: 전송 받을 URL
- method="GET" -> url에 입력값 나타냄
- method="POST" -> url에 입력값 나타내지 않음


# Input 태그
: 사용자에게 입력 받을 데이터 양식

![image](https://user-images.githubusercontent.com/67450413/120432255-a08c2200-c3b4-11eb-962f-ddcaf20989ea.png)
![image](https://user-images.githubusercontent.com/67450413/120432313-bac60000-c3b4-11eb-9a33-aef16c32b09b.png)


# Input 태그의 type 속성
: 입력 데이터의 형식을 정해 줍니다.
ex) <input type="some thing">

![image](https://user-images.githubusercontent.com/67450413/120432775-58b9ca80-c3b5-11eb-9428-9cf06cf2f7c5.png)
![image](https://user-images.githubusercontent.com/67450413/120432836-6ff8b800-c3b5-11eb-91b7-bd7f9fed1c3a.png)

# label 태그
: 제목 요소를 만드는 태그이다.
```html
<input type="checkbox" id="user-agreement" />
<label for="user-agreement">동의하십니까?</label>


<label><input type="checkbox" />동의하십니까?</label>
```
- 위의 두개는 같은 기능을 한다.
- `동의 하십니까?` 라는 텍스트 클릭시 checkbox에 체크 표시됨

# textarea
: 여러 줄의 일반 텍스트 양식이다.
- 텍스트 박스를 만들 수 있고, `placeholder` 속성을 이용하여 hint를 만들어 낼 수 있다!
- hint란 텍스트 박스 입력 전에 미리 나타나 있는 글자를 말하며 클릭 시 사라진다.

# fieldset, legend 태그
: 같은 목적의 양식을 그룹화(fielset)하여 제목(legend)을 지정해 준다.
```html
<form>
  <fieldset>
    <legend>Coffee Size</legend>
    <label>
        <input type="radio" name="size" value="tall" />
        Tall
    </label>
    <label>
        <input type="radio" name="size" value="grande" />
        Grande
    </label>
    <label>
        <input type="radio" name="size" value="venti" />
        Venti
    </label>
  </fieldset>
</form>
```

![image](https://user-images.githubusercontent.com/67450413/120490769-a523fb00-c3f3-11eb-9448-6d6da4276760.png)
- fieldset: 겉 테두리 만들어 줌
- legend: 제목 즉, coffee size 부분에 해당함

# select, datalist, optgroup, option 태그
```html
  <select>
  <optgroup label="Coffee">
    <option>Americano</option>
    <option>Caffe Mocha</option>
    <option label="Cappuccino" value="Cappuccino"></option>
  </optgroup>
  <optgroup label="Latte" disabled>
    <option>Caffe Latte</option>
    <option>Vanilla Latte</option>
  </optgroup>
  <optgroup label="Smoothie">
    <option>Plain</option>
    <option>Strawberry</option>
    <option>Banana</option>
    <option>Mango</option>
  </optgroup>
</select>
```




