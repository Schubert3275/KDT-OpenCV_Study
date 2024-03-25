## OpenCV 딥러닝

<details>
<summary>사용 교재</summary>

![](./images/파이썬으로%20만드는%20OpenCV%20프로젝트.png)

</details>

### DAY01

---

<details>
<summary> Computer Vision </summary>

> -   디지털 이미지나 비디오에서 정보 추출/해석하여 특정 작업 수행
> -   이미지 개선 및 변형
> -   패턴 인식
> -   객체 인식 및 추적
> -   객체 및 영역 분할

</details>
<details>
<summary> Digital Image Processing </summary>

> -   디지털 이미지 신호 처리
> -   전처리 알고리즘
> -   노이즈 및 디노이즈
> -   특징 및 유사성 검출
> -   특징 매칭

</details>
<details>
<summary> Image 구성요소 </summary>

> -   너비(Width/Column/X) & 높이(Height/Row/Y)
> -   정밀도(Bit Depth)
> -   채널(Channel)
> -   색공간(Color Space)
> -   관심영역(ROI: Region Of Interest)
> -   관심채널(COI: Channel Of Interest)
> -   히스토그램

</details>
<details>
<summary> struct 모듈 </summary>

> -   C언어의 struct를 구현한 모듈
> -   바이너리 데이터 처리

</details>
<details>
<summary> os 모듈 </summary>

> -   경로, 파일, 폴더 등등 운영체제 시스템, 파일 시스템 관련 함수, 클래스 제공
> -   폴더 내 모든 폴더 및 파일 리스트 추출 os.listdir
> -   폴더 내 특정 확장자 파일 리스트 추출 os.path.splitext

</details>

---

| 파일명                       | 내용                   |
| ---------------------------- | ---------------------- |
| `DAY_01\ex_mnist_data.ipynb` | Row 이미지 데이터 추출 |
| `DAY_01\ex_dir_path.ipynb`   | os 모듈 활용           |
| `DAY_01\ex_numpy.ipynb`      | 넘파이 기초            |

#### DAY01 실습과제

---

    1. 알파벳 빈도를 통해서 입력 문장의 언어 분석

### DAY02

---

<details>
<summary> OpenCV 기본 함수 </summary>

> -   이미지 데이터 읽기 : cv2.imread()
> -   이미지 창 출력 : cv2.imshow()
> -   이미지 창 제어 : cv2.waitKey(), cv2.destroyAllWindows()
> -   이미지 데이터 저장 : cv2.imwrite()
> -   이미지 데이터 채널 분리 : cv2.split()
> -   이미지 데이터 채널 병합 : cv2.merge()
> -   이미지 색 공간 변환 : cv2.cvtColor()
> -   이미지 크기 변경 : cv2.resize()

</details>
<details>
<summary> 그리기 함수 </summary>

> -   선 그리기 함수 : cv2.line()
> -   사각형 그리기 함수 : cv2.rectangle()
> -   다각형 그리기 함수 : cv2.polylines()
> -   원 그리기 함수 : cv2.circle()
> -   타원 그리기 함수 : cv2.ellipse()
> -   글자 쓰기 함수 : cv2.putText()

</details>
<details>
<summary> 얼굴인식 </summary>

> -   객체 인식 모델 로딩 : cv2.CascadeClassifier.load()
> -   객체 검출 : cv2.CascadeClassifier.detectMultiScale()

</details>
<details>
<summary> CNN </summary>

> -   합성곱신경망(Convolutional Neural Network) : 이미지 분류, 인식, 검출 등 이미지 기반 분야 활용
> -   커널/필터/마스크 : 이미지 위에서 일정 간격으로 이동하며 특징을 추출
> -   스트라이드 : 커널의 이동 방향 및 크기
> -   패딩 : 커널 이미지 외곽 보완 방법

</details>
<details>
<summary> Convolution Layer </summary>

> -   Conv1D : 커널 필터가 좌우로 이동
> -   Conv2D : 커널 필터가 2차원 평면에서 이동
> -   Conv3D : 커널 필터가 3차원 형태로 이동

</details>
<details>
<summary> Polling Layer </summary>

> -   합성곱 층(합성곱 연산 + 활성화 함수) 다음에 풀링 층 추가
> -   다운샘플링으로 특성 맵의 크기를 줄임

</details>

---

| 파일명                      | 내용              |
| --------------------------- | ----------------- |
| `DAY_02\ex_cv_1.ipynb`      | OpenCV 실습       |
| `DAY_02\ex_CIFAR_CNN.ipynb` | CIFAR_10 CNN 학습 |

#### DAY02 실습과제

---

    1. MNIST CNN 학습

### DAY03

---

<details>
<summary> Conv2d </summary>

> -   kernel_size
> -   stride
> -   padding

</details>
<details>
<summary> MaxPool2d </summary>

> -   kernel_size
> -   stride

</details>
<details>
<summary> DataLoader </summary>

> -   batch_size
> -   shuffle
> -   drop_last
> -   sampler

</details>

---

| 파일명                         | 내용                      |
| ------------------------------ | ------------------------- |
| `DAY_03\ex_CNN.ipynb`          | CNN 레이어 분석           |
| `DAY_03\ex_iris_dataset.ipynb` | iris 데이터셋, 데이터로더 |
| `DAY_03\ex_pillow.ipynb`       | pillow 활용               |

#### DAY03 실습과제

---

    1. 동물 이미지 분류
