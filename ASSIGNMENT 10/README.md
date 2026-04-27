# Assignment 10: Rust I/O Models

## Q1 Synchronous I/O
Implemented blocking sequential tasks where each operation completes before the next begins.

Observation:
- Total runtime approximately 1.5 seconds.
- Tasks executed one after another.

---

## Q2 Asynchronous I/O
Implemented asynchronous concurrent tasks using Rust async concepts.

Observation:
- Tasks run concurrently.
- Runtime reduced to approximately 0.5 seconds.

---

## Q3 Polling vs Interrupt
Compared:
- Polling approach
- Interrupt-driven approach

Result:
Interrupt handling is more efficient than continuous polling.

---

## Q4 Vectored I/O
Used vectored writes to send multiple buffers in one operation.

Result:
Improved I/O efficiency.

---

## Q5 Buffered vs Unbuffered
Compared buffered and unbuffered writes.

Result:
Buffered writes performed significantly faster.

---

## Q6 Signal Driven I/O
Implemented signal handling (SIGINT simulation).

Result:
Program responds gracefully to interrupts.
