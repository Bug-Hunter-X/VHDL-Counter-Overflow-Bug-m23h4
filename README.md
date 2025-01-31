# VHDL Counter Overflow Bug
This repository demonstrates a common bug in VHDL code: an integer overflow in a counter. The `buggy_counter.vhdl` file contains a counter that has a potential overflow issue.  The `fixed_counter.vhdl` file shows the corrected code.

## Bug Description
The `buggy_counter` entity uses an integer type to represent the counter value.  If the counter reaches its maximum value (15 in this case), the next increment will cause an overflow. The current implementation doesn't handle this explicitly, potentially leading to unexpected behavior or simulation errors.

## Solution
The `fixed_counter.vhdl` file shows a corrected version of the counter.  This version explicitly handles the overflow condition and resets the counter to 0 when it reaches its maximum value, ensuring correct functionality.
