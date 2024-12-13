FROM python:3.10-slim



# 작업 디렉토리를 /app으로 설정합니다.
WORKDIR /app

# 필요한 패키지를 설치합니다.
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 애플리케이션 코드를 복사합니다.
COPY . .

# 서버를 실행합니다.
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
