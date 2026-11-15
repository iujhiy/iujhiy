<h1 align="center">Nikita Zerkalev</h1>
<h2 align="center">Junior Backend Developer (Java)</h2>

---

## 🎯 About Me
3rd-year student at NRU MPEI. Built from scratch the backend of an information system (Java 21, Spring Boot 3, PostgreSQL): from database design to CI/CD.
Looking for my first commercial backend role to grow in the Spring ecosystem.

---

## 🚀 Featured Project

### Teacher Activity Accounting System
*In development, customer: BIT Department, NRU MPEI · 2026 – present · code available on request*

Backend for tracking and paying for university teachers' activities. 4 roles: teacher, head of department, accountant, administrator.

- Designed a PostgreSQL schema of **14 tables**: employees, departments, substitutions, activities, payments, receipts, reference data, budgets, audit.
- Implemented the full payment lifecycle: activity creation, approval checked against the department's annual budget, accountant review, partial payments across multiple receipts.
- Set up JWT authentication with Spring Security OAuth2 Resource Server and RSA-signed tokens (Nimbus). Wrote two custom filters: dynamic role switching based on an active substitution, and a forced password change.
- Eliminated N+1 with batch fetching and `@EntityGraph` (payment loading: **up to 39 SQL queries → 1**), choosing the strategy based on measurements. Disabled open-in-view.
- Replaced a loop of 50 queries with a single aggregate query: per-teacher totals are **5× faster** (10.9 → 2.1 ms).
- Built dynamic filtering with pagination on 8 Spring Data Specifications.
- Implemented a user action audit log with change history and filtering.
- Wrote **~870 tests** in 139 classes (JUnit 5, Mockito, MockMvc, Spring Security Test, Instancio). JaCoCo coverage: **97% lines, 83% branches**.
- Set up CI/CD on GitLab CI: build, tests, Checkstyle (Sun), JaCoCo, SonarCloud analysis on merge requests and master.

---

## 🛠️ Skills

**Languages**
- Java 21, SQL, C++ (basic)

**Frameworks & Libraries**
- Spring Boot 3.5, Spring MVC, Spring Data JPA, Hibernate 6, Spring Security (OAuth2 Resource Server, JWT), Bean Validation, MapStruct, Lombok, Jackson, Javalin

**Databases**
- PostgreSQL, JPQL, H2 (tests), Redis

**Testing & Quality**
- JUnit 5, Mockito, MockMvc, AssertJ, Spring Security Test, Instancio, integration tests, JaCoCo, Checkstyle, SonarCloud / SonarQube

**DevOps & Tools**
- Git, GitLab CI, GitHub Actions, Gradle (Kotlin DSL), Docker (basic), Linux/Bash, deployment on Render

**API & Monitoring**
- REST API, Swagger/OpenAPI (springdoc), Sentry

**Architecture**
- Layered architecture (Controller → Service → Repository), DTO and mapping (MapStruct), DAO

---

## 🎓 Education

**National Research University "MPEI" (NRU MPEI), Moscow** · 2024–2028
Bachelor's, Applied Informatics in Economics (09.03.03), in progress

**Course projects:**
- **Transport distribution algorithm** – C++, C#
- **Library system database** – designed in Oracle Data Modeler, deployed on PostgreSQL

**Hexlet** · 2025
Profession "Java Developer"

**VTB Named Grants** · 2026
Competition participant, selection in progress

---

## 📌 Work Format
20–30 hours/week, remote or hybrid. Open to project-based collaboration.
English: A2 (reading technical documentation).

---

## 📫 Contact
- **Email:** [nikitazerkalev@gmail.com](mailto:nikitazerkalev@gmail.com)
- **Telegram:** [@Nikita_Zerkalev](https://t.me/Nikita_Zerkalev)
