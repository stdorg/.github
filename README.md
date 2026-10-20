# `stdorg` — Small components. Clear contracts. Composable software.

`stdorg` is a free and open-source initiative focused on building, sharing, and maintaining reusable Go libraries and tools that make software clearer, more reliable, and easier to maintain.

Our repositories form an ecosystem of focused projects designed to be independently useful while remaining open to meaningful integration through shared abstractions and consistent engineering practices.

[**Website**](https://stdorg.github.io) · [**Repositories**](https://github.com/orgs/stdorg/repositories) · [**Discussions**](https://github.com/orgs/stdorg/discussions)

## Engineering Principles

- **Single responsibility** — each component has a clear purpose and a well-defined scope.
- **Explicit contracts** — interfaces and behavior should be predictable, documented, and testable.
- **Composability** — components should integrate naturally when their semantics and contracts align.
- **Maintainability** — favor readable implementations and deliberate design over unnecessary complexity.
- **Extensibility** — allow new capabilities without forcing unrelated components into the same abstraction.
- **Continuous learning** — use experimentation, testing, and iteration to improve engineering practices.

## Project Ecosystem

Projects are organized by responsibility rather than forced into a single framework. Each repository can evolve independently while sharing abstractions where they provide genuine value.

### Access Control

Implementations of distinct authorization models.

- [`role-based-access-control`](https://github.com/stdorg/role-based-access-control) — Role-Based Access Control (RBAC) with role hierarchies, permission assignment, and authorization policies.
- [`attribute-based-access-control`](https://github.com/stdorg/attribute-based-access-control) — Attribute-Based Access Control (ABAC) using subject, resource, action, and environmental attributes.
- [`discretionary-access-control`](https://github.com/stdorg/discretionary-access-control) — Discretionary Access Control (DAC) with resource ownership and owner-managed permissions.
- [`mandatory-access-control`](https://github.com/stdorg/mandatory-access-control) — Mandatory Access Control (MAC) with centrally enforced policies, security labels, and classification levels.

### Data Structures

- [`collections`](https://github.com/stdorg/collections) — Collection data structures and interfaces in Go, inspired by the Java Collections Framework and adapted to Go's type system and idioms.

### Concurrency and Resource Management

- [`object-pool`](https://github.com/stdorg/object-pool) — Object reuse and resource lifecycle management through pooling.
- - [`object-storage`](https://github.com/stdorg/object-storage) — Abstractions for storing, retrieving, and managing objects across storage backends.
- [`worker-pool`](https://github.com/stdorg/worker-pool) — Bounded concurrent task execution, workload distribution, and graceful shutdown.
- [`rate-limiter`](https://github.com/stdorg/rate-limiter) — Configurable rate-limiting policies for controlling throughput and resource consumption.
- [`file-lock`](https://github.com/stdorg/file-lock) — File locking for coordinating access to shared files across concurrent processes.

### Parsing and Language Processing

- [`lexer`](https://github.com/stdorg/lexer) — Lexical analysis and tokenization based on configurable rules.
- [`parser`](https://github.com/stdorg/parser) — Parsing abstractions and utilities for transforming structured input according to defined grammars.
- [`json-parser`](https://github.com/stdorg/json-parser) — JSON parsing, structured value representation, syntax validation, and error reporting.
- [`cli-parser`](https://github.com/stdorg/cli-parser) — Command-line argument parsing for options, positional arguments, subcommands, and validation.
- [`markdown-parser`](https://github.com/stdorg/markdown-parser) — Markdown parsing into structured syntax trees.

### Routing and Dispatch

- [`router`](https://github.com/stdorg/router) — Generic routing abstractions for matching inputs to handlers through configurable rules and dispatch strategies.

### Validation and Templates

- [`schema-validator`](https://github.com/stdorg/schema-validator) — Validation of structured data against declared types, constraints, and rules.
- [`template-engine`](https://github.com/stdorg/template-engine) — Template rendering with variable interpolation, expression evaluation, and reusable templates.

### Filesystem and Error Handling

- [`file-watcher`](https://github.com/stdorg/file-watcher) — File and directory monitoring with filesystem event reporting.
- [`error-context`](https://github.com/stdorg/error-context) — Error enrichment with contextual information while preserving original causes.

## How the Ecosystem Fits Together

Related projects may share interfaces, conventions, or internal utilities when doing so improves interoperability without compromising their individual responsibilities.

Shared abstractions should emerge from stable semantic contracts, not from superficial similarities. Independent components should remain independent when that produces a clearer design.

## Contributing

Contributions should improve correctness, clarity, usability, or maintainability.

1. Read the target repository's README and contribution guidelines.
2. Open an issue or discussion for significant changes before implementation.
3. Keep APIs explicit and focused on the component's responsibility.
4. Include tests for new behavior and regression cases.
5. Document relevant design decisions, limitations, and compatibility considerations.

Each repository may define additional development, testing, and release requirements.

---

<sub>Built in the open through experimentation, deliberate design, and continuous improvement.</sub>
