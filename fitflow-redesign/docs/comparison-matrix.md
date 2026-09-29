# FitFlow Technology Comparison Matrix

## Scoring Method

Scores are project-specific estimates, not benchmark results.

- 1 = Weak fit
- 2 = Below average
- 3 = Adequate
- 4 = Strong
- 5 = Very strong

Weighted total = sum(score × percentage weight) / 100.

## Criteria and Weights

| Code | Criterion | Weight |
|---|---|---|
| P | Performance | 15% |
| S | Scalability | 10% |
| D | Development speed | 20% |
| Sec | Security controls | 20% |
| C | Total cost | 10% |
| AI | AI and ML support | 10% |
| M | Maintainability | 10% |
| X | Cross-platform and real-time integration | 5% |
| | Total | 100% |

Development speed and security receive the highest weights.
FitFlow needs timely improvements while protecting personal data.

Basic iOS, Android and web coverage is also a mandatory requirement.

## Frontend

| Option | P | S | D | Sec | C | AI | M | X | Total |
|---|---|---|---|---|---|---|---|---|---|
| **React Native + Web** | 4 | 4 | 5 | 4 | 4 | 4 | 4 | 5 | **4.25** |
| Flutter | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 5 | 4.05 |
| Kotlin Multiplatform | 5 | 4 | 3 | 4 | 3 | 4 | 3 | 4 | 3.75 |
| SwiftUI-led clients | 5 | 4 | 2 | 4 | 2 | 5 | 2 | 2 | 3.35 |

React Native leads under the assumed React and TypeScript skill base.
SwiftUI-led clients would require additional Android and web technologies.

## Main Backend

| Option | P | S | D | Sec | C | AI | M | X | Total |
|---|---|---|---|---|---|---|---|---|---|
| **Express** | 4 | 4 | 5 | 4 | 4 | 4 | 4 | 4 | **4.20** |
| NestJS | 4 | 4 | 4 | 4 | 4 | 4 | 5 | 4 | 4.10 |
| FastAPI | 4 | 4 | 4 | 4 | 4 | 5 | 4 | 4 | 4.10 |
| Go | 5 | 5 | 3 | 4 | 4 | 3 | 3 | 4 | 3.85 |

Express is selected for the main API.
FastAPI is selected separately for the AI service.

## Database

| Option | P | S | D | Sec | C | AI | M | X | Total |
|---|---|---|---|---|---|---|---|---|---|
| **Firestore** | 4 | 5 | 5 | 4 | 4 | 4 | 4 | 5 | **4.35** |
| PostgreSQL | 5 | 4 | 3 | 5 | 4 | 5 | 4 | 3 | 4.20 |
| MongoDB | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4.00 |
| DynamoDB | 5 | 5 | 3 | 5 | 3 | 4 | 3 | 3 | 4.00 |

Firestore is selected for delivery speed and real-time integration.
PostgreSQL is a strong alternative for relational queries and reporting.

## Authentication

| Option | P | S | D | Sec | C | AI | M | X | Total |
|---|---|---|---|---|---|---|---|---|---|
| **Firebase Auth** | 4 | 5 | 5 | 4 | 4 | 4 | 4 | 5 | **4.35** |
| Cognito | 4 | 5 | 3 | 5 | 4 | 4 | 3 | 4 | 4.00 |
| Auth0 | 4 | 5 | 4 | 5 | 3 | 4 | 4 | 4 | 4.20 |
| Supabase Auth | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4.00 |

AI support here means suitability for protecting and integrating
AI-enabled application services, not model execution.

## Sensitivity Analysis

If React Native's development-speed score falls from 5 to 4,
its total becomes 4.05, tying Flutter.

If 10 percentage points move from development speed to security:
- PostgreSQL rises to 4.40.
- Firestore falls to 4.25.

The recommendation should be reviewed if team skills or governance
requirements change.

Security scores do not establish regulatory compliance.

## Source

Scores and assumptions match the Lab Exercise 05 report.
See lab05-report.docx for detailed comparisons and references.