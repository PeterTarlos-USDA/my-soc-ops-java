# Project Guidelines

## Mandatory Development Checklist
- Lint/diagnostics: check VS Code Problems and fix issues introduced by the change.
- Build: run `cd socops && ./mvnw clean package` before finalizing code changes.
- Test: run `cd socops && ./mvnw test` for Java logic, controller, or behavior changes.
- On Windows PowerShell, use `./mvnw.cmd` if `./mvnw` is not executable.

## Project Shape
- Soc Ops is a Java 21 Spring Boot 3.4.2 social bingo app; runnable code lives in `socops/`.
- Keep app changes in `socops/src/main`; do not edit generated output under `socops/target`.
- `docs/` and `workshop/` contain documentation and lab material.

## Architecture and Style
- `com.socops.model` uses small immutable records/enums; `IcebreakerPrompts` is the inclusive, low-stakes prompt catalogue.
- `BoardAssembler` is pure static board logic; keep behavior side-effect-free and mirror its rules in `templates/game.html` JavaScript.
- `BingoRestController` serves the Thymeleaf page and JSON board endpoint; preserve public routes unless asked.
- Use explicit social-bingo domain names, Java 21 where helpful, and JUnit 5 tests with descriptive `@DisplayName` values.

## Frontend and Change Practices
- Use Thymeleaf, plain JavaScript, and utility classes from `static/css/app.css`; do not add a SPA framework for small UI work.
- When adding CSS, keep utility specificity low and follow `.github/instructions/css-utilities.instructions.md`.
- For larger visual redesigns, also follow `.github/instructions/frontend-design.instructions.md`.
- Add/update tests for board assembly, flipping, victory detection, or controller contract changes.
- Keep board prompt counts aligned: a 5x5 board requires 24 prompts plus the center free cell.