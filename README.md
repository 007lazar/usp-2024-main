USP 2024 – Backend Architecture Demo (.NET)

A clean, modular .NET backend solution demonstrating real-world architecture practices such as separation of concerns, background workers, automated CI, and testable application design.

This repository serves as a backend foundation for a full-stack application and as a portfolio project for software engineering roles.

📌 Why this project exists

This project was built to demonstrate:

Professional multi-project .NET solution design

Clean layering (API, Application, Domain, Infrastructure)

Background processing using worker services

Automated CI with GitHub Actions

Testable, maintainable code structure

🏗 Architecture
USP.sln
├── USP.API              # HTTP API (entry point)
├── USP.Application      # Application logic / use cases
├── USP.Domain           # Core domain models & interfaces
├── USP.Infrastructure  # Data access & external services
├── USP.Worker           # Background / async processing
├── USP.UnitTests        # Unit tests
├── USP.BaseTests        # Shared test utilities
└── .github/workflows    # CI pipelines (GitHub Actions)

Key design principles

Separation of concerns

Dependency inversion

Testability

Scalability

Maintainability

⚙️ Tech stack

C# / .NET

ASP.NET Core

GitHub Actions (CI)

xUnit (unit testing)

Background worker services

🚀 Setup

Restore dependencies, build the solution, and run tests:

dotnet restore
dotnet build
dotnet test

Run API
dotnet run --project USP.API

Run Worker
dotnet run --project USP.Worker

Testing
dotnet test

🔄 Continuous Integration (CI)

This repository uses GitHub Actions to automatically:

Restore dependencies

Build the solution

Run all tests

Every push and pull request is validated automatically.

The CI badge at the top of this README reflects the current build status.

👤 Author

Lazar Milovanovic
Junior Software Engineer
Software & Information Engineering student
Actively seeking junior software engineering roles

GitHub: https://github.com/007lazar

LinkedIn: https://www.linkedin.com/in/lazar-milonvanovic-14b487187

📄 License

MIT
