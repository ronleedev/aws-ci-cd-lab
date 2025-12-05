# Spring Boot EC2 CI/CD Demo

GitHub → CodePipeline → CodeBuild → CodeDeploy → EC2(in-place) 데모.
배포 후 웹 페이지(http://<EC2_IP>:8080)에서 커밋 해시와 빌드 시간이 즉시 바뀝니다.

## Quick Start
1) EC2 보안그룹에 8080 오픈, CodeDeploy Agent 설치/실행
2) CodeDeploy 앱/배포그룹(EC2 태그 기반) 생성
3) CodePipeline(Source=GitHub, Build=CodeBuild, Deploy=CodeDeploy) 구성
4) GitHub에 커밋/푸시 → 파이프라인 완료 후 접속: http://<EC2_PUBLIC_IP>:8080

## CI/CD 흐름 이미지 추가
<img width="1836" height="812" alt="image" src="https://github.com/user-attachments/assets/f2604d24-c1fa-42bb-b050-ea493c1d165c" />
<img width="1801" height="761" alt="image" src="https://github.com/user-attachments/assets/4ba4f636-50f7-40ee-8185-d7ee4946571d" />
<img width="1831" height="800" alt="image" src="https://github.com/user-attachments/assets/aee4ff4f-6931-46c9-b71b-2c8072e13bb5" />
