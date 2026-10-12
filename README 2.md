 Steganography-
 Byte Cybersecurity - Task 02: Steganography

 Objective
Analyze and repair a corrupted PNG file to reveal the hidden flag in the format `flag{...}`.

Tools Used
- Hex Editor (e.g., HxD or Hexyl) to inspect file magic bytes and headers.
- Python for automation and file verification.

Approach
1. Downloaded the corrupted PNG file.
2. Checked file headers to identify corruption (e.g., missing or modified PNG magic numbers).
3. Repaired the file header/chunks and extracted the flag.
