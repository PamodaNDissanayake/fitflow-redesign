# FitFlow Technology Stack

## Selected Technologies

| Layer | Technology | Reason |
|---|---|---|
| Mobile frontend | React Native and TypeScript | Shared Android/iOS development and alignment with the case study |
| Web frontend | React Native Web | Reuse compatible interface components and application logic |
| Main backend | Node.js and Express | Rapid API development using the same TypeScript skills |
| Database | Cloud Firestore | Managed document storage and real-time updates |
| Authentication | Firebase Authentication | Managed identity integrated with Firebase services |
| AI microservice | Python and FastAPI | Separate model inference from the main application API |
| Mobile ML | LiteRT and ML Kit | Support suitable on-device models |
| Cache | Redis when required | Shared rate-limit counters and short-lived template caching |
| Image storage | Private object storage | Store explicitly uploaded images with restricted access |

## Project Requirements

The stack supports:

- Personalized workout plans with understandable explanations.
- Private social circles and community challenges.
- Camera-assisted nutrition logging with manual correction.
- Progress dashboards.
- Offline workout access and later synchronization.

## Assumptions

The comparison assumes a mid-sized team with stronger React
and TypeScript familiarity than Dart, Kotlin or Swift.

This is a planning assumption, not a measured team skill profile.

The academic prototype will use synthetic demonstration data.

## Trade-offs

- Native camera, storage and ML integrations need platform adapters.
- React Native Web does not support every native package automatically.
- Firestore requires index planning and usage-cost monitoring.
- Complex relational reporting may justify PostgreSQL later.
- Python introduces a second backend language to maintain.
- Food recognition requires a suitable model and nutrient data source.

## Security

Firebase Authentication identifies users.
API checks and Firestore Security Rules enforce authorization.

No framework or cloud service makes the application automatically
HIPAA- or GDPR-compliant. A regulated deployment requires a separate
review of data handling, agreements and eligible services.

## Source

See lab05-report.docx for the full comparisons, justifications
and supporting references.