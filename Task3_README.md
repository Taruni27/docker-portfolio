## CI/CD Pipeline

This project uses GitHub Actions for CI/CD automation.

### Workflow:
- On every push to main branch
- Docker image is built automatically
- Image is pushed to Docker Hub

### Tools Used:
- GitHub Actions
- Docker Hub

### Screenshots

<img width="1527" height="298" alt="Docker yml" src="https://github.com/user-attachments/assets/48fa6221-fbeb-4f2b-b674-9ad73afa39f9" />

<img width="1465" height="554" alt="Docker_Build_Steps" src="https://github.com/user-attachments/assets/dca372ff-4abc-4431-8391-be87765a39b6" />

<img width="1569" height="291" alt="Docker_Hub_Repo" src="https://github.com/user-attachments/assets/234a3940-0587-4c96-91ab-2b2f472cf258" />

<img width="1457" height="127" alt="Docker_Completed_Build" src="https://github.com/user-attachments/assets/f06283c1-4b75-40b2-a74b-9787e031cda7" />



### Workflow File:
.github/workflows/docker.yml
