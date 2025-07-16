# String Copy Functions in C — Comparison Table

| Feature                              | `strcpy(dest, src)`                        | `strncpy(dest, src, n)`               | `strlcpy(dest, src, size)` *(non-standard)*                |
| ------------------------------------ | ------------------------------------------ | ------------------------------------- | ---------------------------------------------------------- |
| **Null terminator copied?**          | ✅ Always                                   | ❌ Only if `src` length < `n`          | ✅ Always (as long as `size > 0`)                           |
| **Null-padding if `src` shorter?**   | ❌ No                                       | ✅ Yes                                 | ❌ No                                                       |
| **Truncates if `src` too long?**     | ❌ No (buffer overflow risk)                | ✅ Yes (may omit `\0`)                 | ✅ Yes (always null-terminates if `size > 0`)               |
| **Requires manual null-terminator?** | ❌ No                                       | ✅ Sometimes (if truncation occurs)    | ❌ No                                                       |
| **Buffer overflow safe?**            | ❌ No                                       | ✅ Yes (if `n` ≤ buffer size)          | ✅ Yes (if `size` ≤ buffer size)                            |
| **Returns**                          | Pointer to `dest`                          | Pointer to `dest`                     | Length of `src` *(allows truncation detection)*            |
| **Standard library?**                | ✅ ANSI C                                   | ✅ ANSI C                              | ❌ Not standard C (but used in BSD, macOS, some Linux)      |
| **Best used when...**                | You are 100% sure the buffer is big enough | You want fixed-size copy with padding | You want safe, efficient string copy with truncation check |
