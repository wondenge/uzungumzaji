# uzungumzaji

cross-platform Golang helpers for reading password input without cgo

This package provides cross-platform Go (#golang) helpers for taking user input
from the terminal while not echoing the input back (similar to `getpasswd`). The
package uses syscalls to avoid any dependence on cgo, and is therefore
compatible with cross-compiling.

## Unicode

Multi-byte unicode characters work successfully on Mac OS X. On Windows,
however, this may be problematic (as is UTF in general on Windows). Other
platforms have not been tested.
