# Github Action & Github Container Registry
## Description
Github Container Registry 사용과 Github Action을 통한 CI 연습
## Step
1. Dockerfile로 이미지 빌드 
2. CI를 위한 GithubAction pipelin 작성
3. Github Container Registry에 자동으로 이미지 Push
## Pipeline
```
code commit & push -> Build Dockerfile -> image -> Push to ghcr.io
```
# Image Usage
### build Dockerfile
docker build -t sample .
### Run Image
docker run --rm -d -p 3000:3000 ghcr.io/namhj94/sample2