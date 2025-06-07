# 기존 omr인식 라이브러리 - OMRChecker
---
## 1. 환경 구축

```bash
# 리포지토리 클론
git clone https://github.com/Udayraj123/OMRChecker.git
cd OMRChecker/

# 의존성 설치
python3 -m pip install --user -r requirements.txt

# OpenCV가 없으면 별도로 설치
pip3 install opencv-python
```

## 2. 샘플 실행

```bash
cp -r ./samples/sample1 inputs/
python3 main.py -i ./samples/sample1


*즉, 샘플을 samples 디렉토리에 구축하고 그걸 실행시킬때 인자로 주면 됩니다*
```

## 3. 사용자 OMR 시트 적용

```bash
# 마우스로 선택지 영역을 지정해 템플릿 생성
python3 main.py --setLayout
```

## 4. 실행

```bash
python3 main.py -i ./inputs -o ./outputs
```
