# ZASM - Assembler and Static Linker for ZVM 2.4

**ZASM** is the official assembler and static linker for the **ZVM 2.4 (Zinc Virtual Machine)**.  
It is written in C/C++ and provides a full pipeline from source assembly to raw executable bytecode, supporting multi-file compilation and debug output for development.

---

## Features

- ✅ Full assembler for **ZVM 2.4** instruction set
- ✅ Static linker (no dynamic linking)
- ✅ Multi-file compilation support
- ✅ Internal debug output with `-v` flag
- ✅ Emits raw executable files (no metadata)
- ❌ No macro system
- ❌ No `.include`, `.extern`, or symbol imports yet
- ❌ No relocation or dynamic call tables

---

## Command Line Usage

```bash
zasm <output> -o <input> [options]
````

### Example

```bash
zasm out -o main.s
```

### Flags

| Flag        | Description                              |
| ----------- | ---------------------------------------- |
| `-v`        | Verbose debug output (compilation trace) |
| `-Wnone`    | Disable all warnings                     |
| `--version` | Show compiler version                    |

> **Note:** Output is a raw binary executable targeting ZVM 2.4. No ELF or structured object format is generated.

---

## Output Format

* **Executable**: Raw ZVM bytecode
* **No call tables**
* **No relocation**
* **No metadata section**

---

## License

**Proprietary License**

* All rights reserved.
* Reverse engineering is **not permitted**.
* Modification or redistribution of the source or binaries is **not allowed**.

---

## Author

**Andres Rodriguez Majin**
*Project Owner and Lead Developer*

Contact: `andresrodriguezmajin@gmail.com`

---

## Version

**ZASM for ZVM 2.4**
Current: `v2.4.x` *(Update this as needed)*
