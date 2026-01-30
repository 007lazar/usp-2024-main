USP 2024 – Backend Architecture Demo (.NET)
A clean, modular .NET backend solution demonstrating real-world architecture practices: separation of concerns, background workers, automated CI, and testable application design.
This repository serves as a backend foundation for a full-stack application and as a portfolio project for software engineering roles.

📌 Why this project exists:
-This project was built to demonstrate:
-Professional multi-project .NET solution design
-Clean layering (API, Application, Domain, Infrastructure)
-Background processing using worker services
-Automated CI with GitHub Actions
-Testable, maintainable code structure

Architecture:
USP.sln
│
├── USP.API              # HTTP API (entry point)
├── USP.Application      # Application logic / use cases
├── USP.Domain           # Core domain models & interfaces
├── USP.Infrastructure  # Data access & external services
├── USP.Worker           # Background / async processing
│
├── USP.UnitTests        # Unit tests
├── USP.BaseTests        # Shared test utilities
│
└── .github/workflows    # CI pipelines (GitHub Actions)

