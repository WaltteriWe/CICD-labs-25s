# Node.js CI/CD Demo

## Own additional features: automatic APIDOC when building git workflow

### Screenshots and link to apidoc created using git workflow artifact.

<img width="3187" height="1747" alt="image" src="https://github.com/user-attachments/assets/a94d4cc8-7c99-4791-8dbb-d7c980ac97bc" />

https://users.metropolia.fi/~walttewe/cicd%20test%20apidocs/ Link to automatically generated apidoc of the API used in this excercise.

### Screenshots of workflow test results:

<img width="3170" height="1429" alt="image" src="https://github.com/user-attachments/assets/53f95d00-d6aa-4943-9554-8c819468738d" />

[![Node.js CI](https://github.com/WaltteriWe/CICD-labs-25s/actions/workflows/node.js.yml/badge.svg)](https://github.com/WaltteriWe/CICD-labs-25s/actions/workflows/node.js.yml)

TypeScript Express API with automated CI/CD pipeline.

## Quick Setup

```bash
git clone https://github.com/WaltteriWe/CICD-labs-25s.git
cd CICD-labs-25s
npm install
mysql -u root -p < db/create-db.sql
cp .env.sample .env
npm run dev
```

## API Endpoints

| Method | Endpoint               | Description      |
| ------ | ---------------------- | ---------------- |
| GET    | `/api/v1/students`     | Get all students |
| POST   | `/api/v1/students`     | Create student   |
| PUT    | `/api/v1/students/:id` | Update student   |
| DELETE | `/api/v1/students/:id` | Delete student   |

## CI/CD Pipeline

- Tests on Node.js 22.x and 24.x
- Automated linting and testing
- Generates API documentation


