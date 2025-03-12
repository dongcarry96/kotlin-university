# 학사관리 시스템

## ERD 및 테이블 설계
![ERD](https://github.com/user-attachments/assets/f1369217-e949-4365-b089-c36daa195112)

## REST API 설계

### 👤 학생 API
| 기능            | 메서드   | 엔드포인트                       |
|-----------------|----------|----------------------------------|
| 학생 회원가입   | `POST`   | `/api/users`                     |
| 학생 로그인     | `POST`   | `/api/users/login`               |
| 학생 정보 조회  | `GET`    | `/api/users/{userId}`            |
| 학생 전체 조회  | `GET`    | `/api/users`                     |
| 학생 정보 수정  | `PUT`    | `/api/users/{userId}`            |
| 학생 삭제       | `DELETE` | `/api/users/{userId}`            |

### 👤 교수 API
| 기능            | 메서드   | 엔드포인트                       |
|-----------------|----------|----------------------------------|
| 교수 등록       | `POST`   | `/api/professors`                |
| 교수 로그인     | `POST`   | `/api/professors/login`          |
| 교수 전체 조회  | `GET`    | `/api/professors`                |
| 교수 정보 조회  | `GET`    | `/api/professors/{professorId}`  |
| 교수 정보 수정  | `PUT`    | `/api/professors/{professorId}`  |
| 교수 삭제       | `DELETE` | `/api/professors/{professorId}`  |

### 강의 API
| 기능            | 메서드   | 엔드포인트                       |
|-----------------|----------|----------------------------------|
| 강의 등록       | `POST`   | `/api/courses`                   |
| 강의 전체 조회  | `GET`    | `/api/courses`                   |
| 강의 상세 조회  | `GET`    | `/api/courses/{courseId}`        |
| 강의 수정       | `PUT`    | `/api/courses/{courseId}`        |
| 강의 삭제       | `DELETE` | `/api/courses/{courseId}`        |
| 학생 강의 신청  | `POST`   | `/api/users/{courseId}`          |
| 학생 강의 조회  | `GET`    | `/api/users/{userId}/{courseId}` |
| 학생 강의 삭제  | `DELETE` | `/api/users/{userId}/{courseId}` |



