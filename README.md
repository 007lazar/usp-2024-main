USP 2024 – Backend Architecture (.NET)
https://github.com/007lazar/usp-2024-main\.github\workflows

A clean, modular .NET backend solution demonstrating real-world architecture practices such as separation of concerns, background workers, automated CI, and testable application design.
This repository serves as a backend foundation for a full-stack application and as a portfolio project for software engineering roles.

🏗 Architecture Overview

USP.API
- Entry point of the application
- Exposes HTTP endpoints
- Handles request validation and response formatting
- Delegates business logic to the Application layer

USP.Application
- Contains application use cases
- Orchestrates domain logic
- Coordinates workflows between services
- Independent from infrastructure concerns

USP.Domain
- Core business models and entities
- Domain interfaces and contracts
- Business rules and invariants
- No dependencies on external frameworks

USP.Infrastructure
- Database access and persistence
- External service integrations
- Implementations of domain interfaces
- Isolated from business logic

USP.Worker
- Background and asynchronous processing
- Long-running or scheduled jobs
- Decoupled from HTTP request lifecycle
- Reusable processing logic

Testing Projects
- USP.UnitTests: Unit tests for application and domain logic
- USP.BaseTests: Shared test utilities and test setup

CI / DevOps
-.github/workflows: GitHub Actions pipelines for automated build and test execution

📌 Why this project exists
- This project demonstrates:
- Professional multi-project .NET solution design
- Clean layering (API, Application, Domain, Infrastructure)
- Background processing using worker services
- Automated CI with GitHub Actions
- Testable, maintainable code structure

Key design principles
- Separation of concerns
- Dependency inversion
- Testability
- Scalability
- Maintainability

⚙️ Tech stack
- C# / .NET
- ASP.NET Core
- GitHub Actions (CI)
- xUnit (unit testing)
- Background worker services

🚀 Setup
- Restore dependencies, build the solution, and run tests:
dotnet restore
dotnet build
dotnet test

- Run API
dotnet run --project USP.API

- Run Worker
dotnet run --project USP.Worker

- Testing
dotnet test

🔄 Continuous Integration (CI)
This repository uses GitHub Actions to automatically:
- Restore dependencies
- Build the solution
- Run all tests
- Every push and pull request is validated automatically.
- The CI badge at the top of this README reflects the current build status.

👤 Author
Lazar Milovanovic
Junior Software Engineer
Software & Information Engineering student
Actively seeking junior software engineering roles

GitHub: https://github.com/007lazar
LinkedIn: https://www.linkedin.com/in/lazar-milonvanovic-14b487187

📄 License

MIT
