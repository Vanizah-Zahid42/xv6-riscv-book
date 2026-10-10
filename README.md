The book is available in HTML form at [https://mit-pdos.github.io/xv6-riscv-book/](https://mit-pdos.github.io/xv6-riscv-book/).

The book is available in PDF form at [https://mit-pdos.github.io/xv6-riscv-book/book.pdf](https://mit-pdos.github.io/xv6-riscv-book/book.pdf).

This edition of the book has been converted to LaTeX.
In order to build it, ensure you have a TeX distribution that contains
the `pdflatex` command. With that, you should be able to build the book
by running `make`, which will clone the OS itself and build the book
to `book.pdf` in the main directory.

Figures are drawn using `inkscape`.
## Kernel Modules

|  #  | Module                        | Type         | Description                                            | Status  |
| :-: | :---------------------------- | :----------- | :----------------------------------------------------- | :-----: |
|  1  | `getppid`                     | System Call  | Returns the parent process's ID                        | Pending |
|  2  | `trace`                       | System Call  | Prints each system call a process makes                | Pending |
|  3  | `sysinfo`                     | System Call  | Reports free memory and number of running processes    | Pending |
|  4  | `freemem`                     | System Call  | Returns the number of free memory pages                | Pending |
|  5  | `getprocsize`                 | System Call  | Returns the memory size of the calling process         | Pending |
|  6  | `setpriority` / `getpriority` | System Call  | Sets and reads a process's priority                    | Pending |
|  7  | `syscount`                    | Kernel/User  | Counts how many times each system call is made         | Pending |
|  8  | `ps`                          | User Program | Lists running processes with PID, state, size and name | Pending |
|  9  | `uptime`                      | User Program | Shows how long the system has been running             | Pending |
| 10  | Boot Banner                   | Kernel       | Shows project and team info when xv6 boots             | Pending |
