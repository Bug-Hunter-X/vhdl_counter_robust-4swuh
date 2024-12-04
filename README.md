# VHDL Counter Bug and Solution
This repository demonstrates a common bug in VHDL counters related to potential overflow and sensitivity to clock glitches. The `buggy_counter.vhdl` file contains the buggy code, while `fixed_counter.vhdl` provides a corrected and more robust version.

## Bug Description
The original `buggy_counter` entity uses a simple `if-elsif` statement within a clocked process to increment a counter. However, it lacks sufficient handling of potential edge cases such as reset and clock glitches. This could lead to unpredictable counter values under certain circumstances.

## Solution
The `fixed_counter` entity addresses this issue with improvements such as:
- Using a more robust reset condition, ensuring that the counter resets reliably.
- Adding additional checks to handle clock glitches more effectively.
- Using a more descriptive and readable code style.

This example highlights the importance of thorough testing and proper handling of edge cases in VHDL designs to avoid potential issues in hardware implementations.