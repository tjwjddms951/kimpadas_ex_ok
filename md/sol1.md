# 문제

<img src=https://i.postimg.cc/9MdwFvBN/image.png, width=600>

첨부된 이미지의 **상단 표**는 직원별 사용 가능한 '언어' 역량을 기록한 데이터셋입니다. 이 데이터를 분석하기 용이하도록 **하단 표**와 같은 형태로 전처리하고자 합니다.

> **[데이터 변환 가이드]**
> 
> 1. **데이터 분리 및 추출** >    '언어' 열의 텍스트를 구분자(`/`)로 분리하여, 전체 데이터에 포함된 **모든 언어 종류를 중복 없이 추출**합니다.
> 
> 2. **이진 행렬(Binary Matrix) 생성** >    추출된 각 언어를 개별 열(Column)로 확장하고, 해당 행의 직원이 보유한 언어에는 **1**, 보유하지 않은 언어에는 **0**을 할당합니다.
> 
> 3. **데이터 통합 및 재구성** >    기존 데이터(이름, 나이 등)와 새로 생성된 이진 행렬을 결합하여, **비정형 문자열이 제거된 정형 데이터셋**을 완성합니다.

---

### **[예제 코드]**

```python
# csv 파일 데이터 프레임으로 불러오기
import pandas as pd

url = 'https://raw.githubusercontent.com/panda-kim/csv_files/main/q_and_a.csv'
df = pd.read_csv(url)
```

---

# 문제 해결 절차

---

### **1단계: 문제 정의 (MRE 구성)**


학습자는 주어진 이미지의 복잡한 데이터를 모두 다루기 전, 문제의 핵심을 관통하는 **최소 재현 예제(MRE: minimal and reproducible example)**를 정의합니다. 이때 주어진 MRE로 바라는 결과인 output까지 테이블로 생성합니다.

<img src=https://i.postimg.cc/kMjXFJBP/image.png, width=600>

> **Tip:** input을 생성하는 코드를 제시해도 좋고, 해당 코드를 AI에게 생성해달라고 요청해도 됩니다.

```python
# input 생성 코드
import pandas as pd

data = [['a1', 'A/B', 'b1'], ['a2', 'B', 'b2'], ['a3', 'A/B/C', 'b3']]
df = pd.DataFrame(data, columns=['col1', 'col2', 'col3'])
