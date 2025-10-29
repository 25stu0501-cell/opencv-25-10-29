# opencv-25-10-29
# 🧠 OpenCV란?

> **OpenCV (Open Source Computer Vision Library)**  
> → 컴퓨터 비전(영상 처리)과 인공지능을 위한 **오픈소스 라이브러리**예요.

---

## 📚 기본 정보

| 항목 | 내용 |
|------|------|
| **이름** | OpenCV (Open Source Computer Vision Library) |
| **주요 언어** | C++, Python, Java 등 |
| **용도** | 이미지 및 동영상 처리, 객체 인식, 얼굴 인식 등 |
| **라이선스** | BSD 오픈소스 라이선스 (무료 사용 가능) |
| **지원 플랫폼** | Windows, macOS, Linux, Android, iOS 등 |

---

## 🔍 주요 기능 요약

| 기능 | 설명 | 예시 |
|------|------|------|
| **이미지 읽기/쓰기** | 파일에서 이미지 열기, 저장하기 | `cv2.imread()`, `cv2.imwrite()` |
| **영상 처리** | 회색조 변환, 블러, 에지 검출 등 | `cv2.cvtColor()`, `cv2.GaussianBlur()` |
| **객체 인식** | 얼굴, 눈, 사물 등 인식 | `CascadeClassifier`, DNN, YOLO 등 |
| **형태 분석** | 외곽선, 면적, 중심 찾기 | `cv2.findContours()` |
| **영상 합성** | 두 이미지 합치기, 마스크 처리 | `cv2.addWeighted()` |
| **비디오 처리** | 카메라에서 실시간 프레임 읽기 | `cv2.VideoCapture()` |

---

## 🧩 간단한 예제 코드

```python
import cv2

# 이미지 불러오기
img = cv2.imread('example.jpg')

# 회색조 변환
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# 이미지 표시
cv2.imshow('Gray Image', gray)
cv2.waitKey(0)
cv2.destroyAllWindows()
