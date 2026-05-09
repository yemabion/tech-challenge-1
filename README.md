# Tech Challenge 1

Flask app + Docker + Terraform + GitHub Actions + AWS ECS Fargate.

## Local run
docker build -t tech-challenge-1 .
docker run -p 3000:3000 tech-challenge-1

Open:
http://localhost:3000

## Terraform
cd infra
terraform init
terraform apply

## GitHub Actions
On push to main, the workflow builds the image, pushes to ECR, and updates ECS.