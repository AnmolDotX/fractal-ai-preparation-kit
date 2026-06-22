This is a comprehensive, end-to-end preparation guide tailored for a **Full-Stack Developer (React + Python + FastAPI)** with **3 years of experience** interviewing at Fractal Analytics.

At the 3-year mark, Fractal expects you to move past syntax and basic implementations. They will evaluate your understanding of production-ready code, performance optimization, system bottlenecks, and clean architectural patterns.

---

## 1. Data Structures & Algorithms (DSA) & SQL

Fractal's technical evaluation frequently pairs a live coding DSA problem with a real-time relational database query scenario.

### Core DSA Topics to Master

* **Arrays & Strings:** Two-pointer approaches, sliding window techniques, and frequency maps.
* **Stacks & Queues:** Monotonic stacks, parenthetical matching, and queue tracking.
* **Linked Lists:** Cycle detection, list reversals, and finding intersection points.
* **Recursion & Hashing:** Memoization approaches and implementing custom hashing lookups.

### Target Interview Questions

* *Given an array of integers representing daily stock prices, find the maximum profit you can achieve by buying and selling once.*
* *Find the length of the longest substring in a given string without repeating characters.*
* *Implement an algorithm to determine if a string has validly balanced parentheses and brackets.*
* *Given an array of intervals representing meetings, determine the minimum number of conference rooms required.*

### SQL & Database Querying Topics

* **Window Functions:** `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, and `LEAD/LAG`.
* **Aggregations & Grouping:** Combining `GROUP BY` with `HAVING` clauses and filtering pre/post aggregation.
* **Complex Joins:** Utilizing `LEFT JOIN`, `INNER JOIN`, and understanding the operational difference between `WHERE` and `ON` clauses.

### Target SQL Questions

* *Write a query to find the top 3 highest-earning employees in each department (requires analytical window functions).*
* *Given a table of user logins with timestamps, find all users who logged in on consecutive days.*

---

## 2. Frontend Architecture (JavaScript & React)

For a mid-level engineer, the frontend loop focuses heavily on component architectural design, state synchronization, and render optimizations.

### Core JavaScript Concepts

* **Asynchronous Engine:** Event Loop, Microtask Queue vs. Macrotask Queue, and execution contexts.
* **Closures & Scoping:** Lexical scoping, memory leaks caused by uncleared event listeners, or persisting references inside closures.
* **Prototypes & Modern Features:** Prototypal inheritance, Prototypal chain, and deep structural copying techniques.

### Core React Concepts

* **Reconciliation & VDOM:** How the Virtual DOM diffing algorithm works, and the critical performance role of the `key` prop.
* **State & Hook Lifecycle:** Component mounting closures, custom hooks encapsulation, and the granular rendering impact of `useEffect`, `useMemo`, and `useCallback`.
* **State Management:** Local component state vs. Global Context API, and handling context-induced re-render bottlenecks.

### Target Frontend Questions

* *Explain how the React rendering lifecycle handles state batches. What happens when you update a state three times sequentially in a single function handler?*
* *Write a custom hook `useFetch` that handles API requests, loading indicators, error handling, and automatically aborts the active request via `AbortController` if the component unmounts mid-flight.*
* *How do you optimize a large React list view containing 10,000 interactive items suffering from visible typing lag? (Expect discussions around virtualization, debouncing, and memoization).*

---

## 3. Backend Engineering (Python & FastAPI)

Fractal will assess your mastery over modern Python paradigms, concurrent execution models, and fast API delivery principles.

### Core Python Concepts

* **Memory & Concurrency:** Global Interpreter Lock (GIL) implications, multi-threading vs. multi-processing use cases, and how `asyncio` handles I/O bottlenecks.
* **Advanced Syntax:** Decorators for cross-cutting concerns, Generators for streaming memory optimization, and Context Managers (`with` blocks).

### FastAPI & API Design Concepts

* **Dependency Injection System:** Building reusable authentication, database session, and rate-limiting middleware injectors.
* **Pydantic Data Layer:** Implementing strict request/response schemas, runtime type validation, and data serialization.
* **Concurrency Models:** When to declare paths with `async def` versus standard synchronous `def` (and how threads execute under worker pools like Uvicorn/Gunicorn).

### Target Backend Questions

* *How does FastAPI achieve high performance relative to older frameworks like Flask or Django? Explain its interaction with ASGI and Uvicorn.*
* *Write a custom Python decorator that metrics the execution time of an API endpoint and logs it if it exceeds a 200ms threshold.*
* *How would you handle a long-running computation task (e.g., generating a massive PDF report) inside a FastAPI application without blocking incoming HTTP client requests?*

---

## 4. System Design & Engineering Architecture

At 3 years of experience, you must demonstrate structural awareness regarding how data flows between your React frontend and FastAPI backend safely and efficiently.

### System Design Topics

* **API Architectures:** Designing intuitive REST endpoints, implementing status codes accurately, pagination patterns (Cursor vs. Offset), and rate limiting.
* **Caching Layers:** Implementing Redis or Memcached strategies for distributed caching, session data management, and dealing with cache invalidation rules.
* **Authentication & Security:** JWT validation mechanics, token-refresh strategies, CORS control headers, and OWASP Top 10 web protections.

### Target System Design Scenarios

* *Design an interactive, real-time dashboard tracking infrastructure resource metrics. How do you decide between WebSockets and Long Polling? How do you structure the ingestion database layer?*
* *Design a secure file-upload profile service where a user uploads an avatar image from a React UI. Explain the workflow using signed URLs directly to S3 vs. routing the payload binary straight through a FastAPI endpoint.*

---

## 5. Behavioral & Cultural Fitment

Fractal emphasizes consulting, data delivery excellence, and cross-functional team collaboration.

* **Handling Technical Debt:** *"Tell me about a project where you had to ship a feature quickly knowing the code structure was imperfect. How did you balance the speed premium versus future technical debt?"*
* **Conflict Resolution:** *"Describe a scenario where you disagreed with a senior engineer or product owner regarding an technical approach or tech stack choice. How did you handle the situation and arrive at a consensus?"*
* **Ambiguity:** *"How do you approach a feature request when the initial requirements sheet from product management is vague or incomplete?"*

### Preparation Checklist

1. **DSA Practice:** Focus heavily on Array, Hashmap, and Stack-based problems using LeetCode (Easy to Medium).
2. **API Hands-on:** Re-verify your conceptual understanding of how FastAPI hooks into its event loop and how to structure production database engines efficiently.
3. **Frontend Deep-Dive:** Be fully ready to explain React performance optimizations out loud while coding on an online canvas.
