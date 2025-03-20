# Collaborative task management application
# System Architecture

                    ┌─────────────────┐
                    │  GitHub Actions │
                    │  CI/CD Pipeline │
                    └────────┬────────┘
                             │
                             ▼
┌─────────────┐     ┌─────────────────┐     ┌───────────────┐
│   Angular   │◄────┤     Quarkus     │◄────┤   PostgreSQL  │
│ Frontend    │     │    Backend      │     │   Database    │
└──────┬──────┘     └────────┬────────┘     └───────────────┘
       │                     │
       │                     │
       │            ┌────────▼────────┐
       └───────────►│      Kafka      │◄───────────┘
                    │  Event Streaming│
                    └─────────────────┘
