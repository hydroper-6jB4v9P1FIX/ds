# To-do

## Code Usage and Analysis

- [ ] Usage counter

## Name resolution

- [ ] Tuple-struct initializer may not be a tuple initializer because of the struct constructor; therefore, defer initializer resolution until it is known whether the direct struct constructor has been provided or not.

## Visibility

- [ ] Visibility is public or a module. The default visibility is the outer module. `pub(qns)` means the module `qns`.
- [ ] Although structs and enums use the same AST, the default visibility for their struct fields and tuple fields is determined differently. For enums, the visibility of content inside is the same as the enum's one.

## Modules

- [ ] Loading the same external source file twice isn't allowed.

## Macros

- [ ] Procedural macros return a `TokenStream` and a collection of diagnostics that the parser accepts.

## Attributes

- Conditional compilation
  - [ ] Key-value pairs are quantified by value (`String = Vec<String>`) since key is not unique.