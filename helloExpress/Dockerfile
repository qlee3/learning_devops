#base images
FROM node:10.15

#Dockerfile 을 생성/관리하는 사람
MAINTAINER Yunkyu Lee <gtv1523411@gmail.com>
# /app 디렉토리 생성
RUN mkdir -p /app
# /app 디렉토리를 WORKDIR 로 설정
WORKDIR /app
# 현재 Dockerfile 있는 경로의 모든 파일을 /app 에 복사
ADD . /app
# npm install 을 실행
RUN npm install

#환경변수 NODE_ENV 의 값을 development 로 설정
ENV NODE_ENV production
ENV PORT 3000

#가상 머신에 오픈할 포트
EXPOSE 3000

CMD [ "npm", "start" ]
