## ✅ **공식 문서 찾는 법**


* 구글에서 **pandas 함수명**을 입력하면 가장 먼저 검색됩니다.
<img src=https://i.postimg.cc/qvc876vr/image.png, width=600>

<br>
 
* 책에서 함수의 페이지를 찾으면 통상적으로 공식 문서의 페이지가 나옵니다.
* 강의 자료에서 **판다스 함수명**을 입력하면 한글 공식 문서를 확인할 수 있습니다.

<br>

* 구글 코랩(Google Colab)에서 함수를 사용 후 `shift + tab`을 입력하면 공식 문서를 불러옵니다.
<img src=https://i.postimg.cc/43NBkQbV/image.png, width=600>


---

## ✅ **공식 문서 읽는 법**

### **1. 웹페이지 활용**

<img src=https://i.postimg.cc/XqMfJfFg/image.png, width=600>

* 구글에서 **pandas 함수명**을 검색하면 웹페이지에서 상세 내용을 확인할 수 있습니다.

---

### **2. 한글 공식 문서 (강의 자료) 활용**

<img src=https://i.postimg.cc/qM4K5MGF/image.png, width=600>

* 강의 자료의 공식 문서는 한글로 되어 있어 개념을 파악하기 쉽습니다.

#### **⭐ 판다스 `pivot_table`**
> 원시 데이터로 피벗 테이블을 생성하는 함수

**`pivot_table` 함수의 주요 매개변수와 인수, 기본값**

```python
df.pivot_table(values=None, index=None, columns=None, aggfunc='mean')
```

* **`values`**: 집계할 대상 열을 지정합니다. (예: 점수 열 집계)
* **`index`**: 행으로 구분할 그룹을 나누는 기준 열을 지정합니다. (예: 반별 구분)
* **`columns`**: 열로 구분할 그룹을 나누는 기준 열을 지정합니다. (예: 성별 구분)
* **`aggfunc`**: 그룹의 차원을 축소할 집계 함수를 지정합니다. 기본값은 `'mean'`으로 그룹의 평균을 구해 차원을 축소합니다.

---

### **3. 구글 코랩 등의 IDE에서 함수를 사용 후 "shift + tab"을 입력**

<img src=https://i.postimg.cc/2ym1M2hP/image.png, width=600>


