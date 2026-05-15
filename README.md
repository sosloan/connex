# connex

Connex is a lightweight specification repository for a Louisiana-themed emoji DSL
for structured parallel stream processing.

## Example program

The repository includes a cleaned example program at
`examples/crawfish_boil.connex`.

## Core operators

| Emoji | Meaning |
| --- | --- |
| `🎈` | allocate shared memory |
| `🔒` / `🔓` | lock / unlock a resource |
| `🎯` | free a resource |
| `🐊` | create a lazy bayou stream |
| `🍲 { ... }` | combine streams or heterogeneous data |
| `🌊 { ... }` | run the main pipeline flow |
| `🎉 ... { ... }` | parallel or broadcast-style execution |
| `🎷 { ... }` | adaptive execution block |
| `🏝️ { ... }` | fork-join distribution |
| `🎭` | spawn an actor |
| `⚜️ fn` | pure function |
| `📬` | send a message |
| `🎂` | circular buffer or token ring operation |

## Semantics

- Streams are lazy by default.
- `⚜️` functions are side-effect free.
- `🏝️` blocks execute branches in parallel and synchronize before exit.
- `🎷` blocks allow runtime-adaptive behavior inside a larger parallel flow.

## Status

This repository currently provides the language concept and a reference example.
