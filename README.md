# BracketStructureParser

This package can be used to parse structures that have a lisp-like brackety hierarchy.

Example usage:

```swift
BracketStructure(string: "(branch hello (branch 2 (leaf 1) (leaf 3)) (leaf 5))")

// Gives the structure:
//
// BracketStructure.container([
//   .text("branch"),
//   .text("hello"),
//   .container([
//     .text("branch"),
//     .text("2"),
//     .container([
//       .text("leaf"),
//       .text("1")
//     ]),
//     .container([
//       .text("leaf"),
//       .text("3")
//     ])
//   ]),
//   .container([
//     .text("leaf"),
//     .text("5")
//   ])
// ])

```
