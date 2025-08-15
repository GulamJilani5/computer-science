☑️✔️🟦🟣🔵🟢🔴🟡🟠➡️⭕🟠⬛🟩🟪🟫 ➡️ ⏺️ ••‣⁎⁕⁜※⁂

# ⏺️ Computer Architecture & Execution Models

## ➡️ Parallel = simultaneous = multiple tasks exactly same time

- **Parallelism** means two or more tasks are literally running at the exact same instant.
  - This requires multiple cores (or multiple CPUs).
  - **Example:** On your laptop, if Core 1 runs Chrome and Core 2 runs Spotify at the same moment, that’s parallel  
    execution.

## ➡️ Concurrency = interleaved or asynchronous or parallel

- Concurrency is about structure and dealing with many things at once, that can be at the same time or not.
- **Concurrency can be:**
  - **Interleaved** One CPU core rapidly switches between tasks (time slicing).
  - **Parallel** Multiple cores truly execute at once.
  - **Asynchronous** Tasks are managed independently, often waiting for I/O operations (**e.g.**, reading a file or network request).

## ➡️ Multithreading = parallel or interleaved

- Multithreading is one way to achieve concurrency
- **If your CPU has multiple cores →** those threads can run in **Parallel**.
- **If your CPU has one core →** threads run **Interleaved** via context switching.

## ➡️ Process vs Thread

### 🟦 Process

A running program with its own memory space and system resources.
Each process is isolated — one process’s memory can’t be directly accessed by another process.

- **Example:**
  - **Process 1:** Google Chrome (has its own memory for tabs, bookmarks, cookies, etc.)
  - **Process 2:** Spotify (its own memory for playlists, audio buffer, etc.)

### 🟦 Thread

A smaller unit of execution inside a process.
Threads in the same process share the process’s memory space but can run independently.

- **Example:**
  - Chrome might have:
    - **Thread 1:** Render tab 1
    - **Thread 2:** Render tab 2 - **Thread 3:** Handle downloads

All these threads share Chrome’s allocated RAM but run independently.
