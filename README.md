## binception: Generate hash values for functions within a binary.

### What
binception is a utility that locates functions within an elf file (library,
executable, object).  The hash values for all discovered functions can
be reported to stdout or saved in a sqlite3 database.

## Why
efh is used to hash the code of functions within an ELF binary.  The goal is to
use this tool to figure out if that same function exists within another binary.

### Dependencies
* binutils: https://www.gnu.org/software/binutils/ (ELF handling)
* sqlite3: https://www.sqlite.org/  (Database functionality)
* openssl: https://www.openssl.org/ (MD5 hashing algo)

### Building
Run *make* from the source directory.  The resulting binary can be copied
anywhere.

### Contact
mattdavis9@gmail.com (enferex)
