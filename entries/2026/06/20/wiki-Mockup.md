---
source: sources/wiki-Mockup.md
source_url: https://en.wikipedia.org/wiki/Mockup
---

## Mockups: Scale and Full-Size Models in Design and Engineering

A mockup is a scale or full-size model of a design or device used for teaching, demonstration, design evaluation, promotion, and testing purposes across many industries. Mockups serve as critical design tools that allow feedback, iteration, and validation before committing to expensive production, spanning fields from manufacturing and military acquisition to software engineering and architecture.

## Key Concepts

- A **mockup** is a scale or full-size model used to evaluate, demonstrate, or test a design before production
- A mockup **may be a prototype** if it provides at least part of the system's functionality and enables testing — but not all mockups are prototypes
- Core purpose: gather user feedback and catch design errors early ("fix it on the drafting board with an eraser, not on the construction site with a sledgehammer")
- Mockups are intentionally **incomplete** — they prioritize speed and cost-effectiveness over finish quality
- In **software engineering**, "mockup" has two distinct meanings:
  - **UI mockups**: visual representations of software interfaces (hand-drawn layouts through semi-functional UIs) that show appearance without underlying functionality
  - **Mock objects**: test doubles used in unit testing to simulate dependencies, enabling isolated testing of individual components
- **Service virtualization** and **API mocks** are "over-the-wire test doubles" used in SOA/microservices architectures
- In **garment-making**, mockups are called **muslins** or **toiles**, made in cheap fabric to test fit and pattern
- In **architecture**, mockups verify material/color selections and can be used for performance testing (e.g., water penetration)
- In **furniture/cabinetry**, full-sized replicas in inexpensive materials verify proportions, ergonomics, and finish

## Commands and Syntax

No specific commands or configuration syntax — this is a conceptual/definitional topic. However, relevant software engineering practices include:

- Creating **mock objects** to replace dependencies in unit tests (frameworks vary by language: Mockito, unittest.mock, Jest mocks, etc.)
- Building **wireframes** as low-fidelity UI mockups before coding
- Using **service virtualization tools** to mock API dependencies in SOA environments

## Relationships

- **Mockup vs. Prototype**: A mockup shows appearance/form; a prototype provides functional behavior. A mockup *becomes* a prototype when it implements partial functionality
- **Mockup vs. Wireframe**: In software/systems engineering, the distinction is blurred — wireframes are a type of low-fidelity mockup
- **Mock objects** relate to **test doubles**, **unit testing**, and **service virtualization**
- **Service-oriented architecture (SOA)** and **microservices** use API mocks to decouple component testing
- Connected design tools: blueprints, CAD, sketches, storyboards, technical drawings, design specifications
- Related to **human factors/ergonomics** testing across military, consumer goods, and furniture domains

## Exam-Relevant Points

- A mockup is NOT always a prototype — it becomes one only when it provides partial system functionality
- In software, **mock objects** serve a different purpose than **UI mockups**: mock objects isolate unit tests by faking dependencies; UI mockups visualize interfaces without backend logic
- Mock objects are especially important when dependencies involve **complex computation** or **non-deterministic results** (e.g., sensor readouts)
- The key value proposition of mockups across all domains is **early error detection** — catching design flaws before expensive production/construction
- In systems engineering, best practice is to **design or prototype the UI before writing source code** or building hardware
- **Service virtualization** is the SOA/microservices equivalent of mock objects, operating "over the wire" via protocols like HTTP
- Mockups are used across: manufacturing, military acquisition, garment-making, consumer goods, furniture, software engineering, and architecture
