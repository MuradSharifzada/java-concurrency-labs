# Java Concurrency Labs: Threads, Multithreading, Parallelism

Hands-on labs to learn Java threading, concurrency, and parallelism from zero to deep. Each module includes tasks, unit tests, and guidance. Each module also has a THEORY.md with advanced notes that go beyond “how” into “why”.

## Prerequisites
- JDK 17+ installed. Module 12 (virtual threads) requires JDK 21+.
- Maven 3.9+ (`mvn -v`)

## How to run
- Run all tests:
  ```bash
  mvn -q -DskipTests=false test
  ```
- Run a single module’s tests:
  ```bash
  mvn -q -pl 01-threads-basics -DskipTests=false test
  ```

## Modules
0. Intro and Java Memory Model overview (this README + THEORY)
1. Threads basics (start/join, lifecycle) — [theory](01-threads-basics/THEORY.md)
2. Synchronization (synchronized, volatile) — [theory](02-synchronization/THEORY.md)
3. Executors (thread pools, tuning) — [theory](03-executors/THEORY.md)
4. Synchronizers (latches, barriers, semaphores, phasers) — [theory](04-synchronizers/THEORY.md)
5. Locks & Atomics (ReentrantLock, RWLock, StampedLock, AtomicX) — [theory](05-locks-and-atomics/THEORY.md)
6. Concurrent Collections — [theory](06-concurrent-collections/THEORY.md)
7. CompletableFuture & async composition — [theory](07-completablefuture/THEORY.md)
8. Parallel Streams — [theory](08-parallel-streams/THEORY.md)
9. Fork/Join — [theory](09-forkjoin/THEORY.md)
10. Cancellation & Interruption — [theory](10-cancellation-and-interruption/THEORY.md)
11. Performance & JMH — [theory](11-performance-jmh/THEORY.md)
12. Virtual Threads (Java 21+) — [theory](12-virtual-threads/THEORY.md)
13. Testing & Debugging Concurrency — [theory](13-testing-and-debugging/THEORY.md)
14. Concurrency Design Patterns — [theory](14-design-patterns/THEORY.md)

## Learning path
1) Read the module README and THEORY.
2) Run tests (`mvn test`) to see failing tasks.
3) Implement code under `src/main/java` to make tests pass.
4) Study “Deep Dive” and pitfalls in each THEORY.md.
5) Optionally document insights or pitfalls you find in module READMEs.

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md)

## License
MIT