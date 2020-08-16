# EPID: Type-C PID controller library

---

## Description

Portable implementation of **Type-C PID controller** for both hosted
and freestanding C environments with a flexible API that allow the usage of
third-party external and/or internal filter(s) for a better control
backed with errors and exceptions handling.

Type-C PID controller equations brief [^fn]:  
`x`: Measured process variable (PV).  
`P[k] = Kp * (x[k-1] - x[k])`  
`I[k] = Ki * e[k] = Ki * (SP - x[k])`  
`D[k] = Kp * (2*x[k-1] - x[k-2] - x[k])`  
`y[k] = y[k-1] + delta[k] = y[k-1] + P[k] + I[k] + D[k]`  

[^fn]: D. M. Auslander, Y. Takahashi and M. Tomizuka, "Direct digital process
control: Practice and algorithms for microprocessor application,"
in Proceedings of the IEEE, vol. 66, no. 2, pp. 199-208, Feb. 1978,
doi: 10.1109/PROC.1978.10870.

---

## Features

- Portable code: C standard ISO/IEC 9899:1999 (C99) or later.
- Usage of IEEE-754 standard for floating-point arithmetic.
- Handling of floating-point arithmetic errors.
- Flexible API by dividing processing functions to allow the usage of
third-party external and/or internal filter(s).
- Permissive free software license (ISC).

---

## Software repository

GitHub repository: <https://github.com/abderraouf-adjal/Embedded-PID>

---

## Copyright and licensing

**File:**  `LICENSE.txt`.