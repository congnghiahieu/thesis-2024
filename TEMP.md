| Order | Class Name                     | Description                                                                                                    |
| ----- | ------------------------------ | -------------------------------------------------------------------------------------------------------------- |
| 1     | Abi                            | The binary interface of a function: `extern "C"`.                                                              |
| 2     | AngleBracketedGenericArguments | Angle bracketed arguments of a path segment: the `<K, V>` in HashMap<K, V>.                                    |
| 3     | Arm                            | One arm of a `match` expression: `0..=10 => { return true; }`.                                                 |
| 4     | AssocConst                     | An equality constraint on an associated constant: `the PANIC = false in Trait<PANIC = false>`.                 |
| 5     | AssocType                      | A binding (equality constraint) on an associated type: `the Item = u8 in Iterator<Item = u8>`.                 |
| 6     | Attribute                      | An attribute, like `#[repr(transparent)]`.                                                                     |
| 7     | BareFnArg                      | An argument in a function type: `the usize in fn(usize) -> bool`.                                              |
| 8     | BareVariadic                   | The variadic argument of a function pointer like `fn(usize, ...)`.                                             |
| 9     | Block                          | A braced block containing Rust statements.                                                                     |
| 10    | BoundLifetimes                 | A set of bound lifetimes: `for<'a, 'b, 'c>`.                                                                   |
| 11    | ConstParam                     | A const generic parameter: `const LENGTH: usize`.                                                              |
| 12    | Constraint                     | An associated type bound: `Iterator<Item: Display>`.                                                           |
| 13    | DataEnum                       | An enum input to a `proc_macro_derive` macro.                                                                  |
| 14    | DataStruct                     | A struct input to a `proc_macro_derive` macro.                                                                 |
| 15    | DataUnion                      | An untagged union input to a `proc_macro_derive` macro.                                                        |
| 16    | DeriveInput                    | Data structure sent to a `proc_macro_derive` macro.                                                            |
| 17    | Error                          | Error returned when a Syn parser cannot parse the input tokens.                                                |
| 18    | ExprArray                      | A slice literal expression: `[a, b, c, d]`.                                                                    |
| 19    | ExprAssign                     | An assignment expression: `a = compute()`.                                                                     |
| 20    | ExprAsync                      | An async block: `async { ... }`.                                                                               |
| 21    | ExprAwait                      | An await expression: `fut.await`.                                                                              |
| 22    | ExprBinary                     | A binary operation: `a + b, a += b`.                                                                           |
| 23    | ExprBlock                      | A blocked scope: `{ ... }`.                                                                                    |
| 24    | ExprBreak                      | A `break`, with an optional label to break and an optional expression.                                         |
| 25    | ExprCall                       | A function call expression: `invoke(a, b)`.                                                                    |
| 26    | ExprCast                       | A cast expression: `foo as f64`.                                                                               |
| 27    | ExprClosure                    | A closure expression: `[a, b] + a + b`.                                                                        |
| 28    | ExprConst                      | A const block: `const { ... }`.                                                                                |
| 29    | ExprContinue                   | A `continue`, with an optional label.                                                                          |
| 30    | ExprField                      | Access of a named struct field `obj.k` or unnamed tuple struct field `obj.0`.                                  |
| 31    | ExprForLoop                    | A for loop: `for pat in expr { ... }`.                                                                         |
| 32    | ExprGroup                      | An expression contained within invisible delimiters.                                                           |
| 33    | ExprIf                         | An if expression with an optional else block: if expr { ... } else { ... }.                                    |
| 34    | ExprIndex                      | A square bracketed indexing expression: vector[2].                                                             |
| 35    | ExprInfer                      | The inferred value of a const generic argument, denoted \_.                                                    |
| 36    | ExprLet                        | A let guard: let Some(x) = opt.                                                                                |
| 37    | ExprLit                        | A literal in place of an expression: 1, "foo".                                                                 |
| 38    | ExprLoop                       | Conditionless loop: loop { ... }.                                                                              |
| 39    | ExprMacro                      | A macro invocation expression: format!("{}", q).                                                               |
| 40    | ExprMatch                      | A match expression: match n { Some(n) => {}, None => {} }.                                                     |
| 41    | ExprMethodCall                 | A method call expression: x.foo::<T>(a, b).                                                                    |
| 42    | ExprParen                      | A parenthesized expression: (a + b).                                                                           |
| 43    | ExprPath                       | A path like std::mem::replace possibly containing generic parameters and a qualified self-type.                |
| 44    | ExprRange                      | A range expression: 1..2, 1.., ..2, 1..=2, ..=2.                                                               |
| 45    | ExprRawAddr                    | Address-of operation: &raw const place or &raw mut place.                                                      |
| 46    | ExprReference                  | A referencing operation: &a or &mut a.                                                                         |
| 47    | ExprRepeat                     | An array literal constructed from one repeated element: [0u8; N].                                              |
| 48    | ExprReturn                     | A return, with an optional value to be returned.                                                               |
| 49    | ExprStruct                     | A struct literal expression: Point { x: 1, y: 1 }.                                                             |
| 50    | ExprTry                        | A try-expression: expr?.                                                                                       |
| 51    | ExprTryBlock                   | A try block: try { ... }.                                                                                      |
| 52    | ExprTuple                      | A tuple expression: (a, b, c, d).                                                                              |
| 53    | ExprUnary                      | A unary operation: !x, \*x.                                                                                    |
| 54    | ExprUnsafe                     | An unsafe block: unsafe { ... }.                                                                               |
| 55    | ExprWhile                      | A while loop: while expr { ... }.                                                                              |
| 56    | ExprYield                      | A yield expression: yield expr.                                                                                |
| 57    | Field                          | A field of a struct or enum variant.                                                                           |
| 58    | FieldPat                       | A single field in a struct pattern.                                                                            |
| 59    | FieldValue                     | A field-value pair in a struct literal.                                                                        |
| 60    | FieldsNamed                    | Named fields of a struct or struct variant such as Point { x: f64, y: f64 }.                                   |
| 61    | FieldsUnnamed                  | Unnamed fields of a tuple struct or tuple variant such as Some(T).                                             |
| 62    | File                           | A complete file of Rust source code.                                                                           |
| 63    | ForeignItemFn                  | A foreign function in an extern block.                                                                         |
| 64    | ForeignItemMacro               | A macro invocation within an extern block.                                                                     |
| 65    | ForeignItemStatic              | A foreign static item in an extern block: static ext: u8.                                                      |
| 66    | ForeignItemType                | A foreign type in an extern block: type void.                                                                  |
| 67    | Generics                       | Lifetimes and type parameters attached to a declaration of a function, enum, trait, etc.                       |
| 68    | Ident                          | A word of Rust code, which may be a keyword or legal variable name.                                            |
| 69    | ImplGenerics                   | Returned by Generics::split_for_impl.                                                                          |
| 70    | ImplItemConst                  | An associated constant within an impl block.                                                                   |
| 71    | ImplItemFn                     | An associated function within an impl block.                                                                   |
| 72    | ImplItemMacro                  | A macro invocation within an impl block.                                                                       |
| 73    | ImplItemType                   | An associated type within an impl block.                                                                       |
| 74    | Index                          | The index of an unnamed tuple struct field.                                                                    |
| 75    | ItemConst                      | A constant item: `const MAX: u16 = 65535`.                                                                     |
| 76    | ItemEnum                       | An enum definition: `enum Foo<A, B> { A(A), B(B) }`.                                                           |
| 77    | ItemExternCrate                | An extern crate item: `extern crate serde`.                                                                    |
| 78    | ItemFn                         | A free-standing function: `fn process(n: usize) -> Result<(), ... }`.                                          |
| 79    | ItemForeignMod                 | A block of foreign items: `extern "C" { ... }`.                                                                |
| 80    | ItemImpl                       | An impl block providing trait or associated items: `impl<A> Trait for Data<A> { ... }`.                        |
| 81    | ItemMacro                      | A macro invocation, which includes `macro_rules!` definitions.                                                 |
| 82    | ItemMod                        | A module or module declaration: `mod m or mod m { ... }`.                                                      |
| 83    | ItemStatic                     | A static item: `static BIKE: Shed = Shed(42)`.                                                                 |
| 84    | ItemStruct                     | A struct definition: `struct Foo<A> { x: A }`.                                                                 |
| 85    | ItemTrait                      | A trait definition: `pub trait Iterator { ... }`.                                                              |
| 86    | ItemTraitAlias                 | A trait alias: `pub trait SharableIterator = Iterator + Sync`.                                                 |
| 87    | ItemType                       | A type alias: `type Result<T> = std::result::Result<T, MyError>`.                                              |
| 88    | ItemUnion                      | A union definition: `union Foo<A, B> { x: A, y: B }`.                                                          |
| 89    | ItemUse                        | A use declaration: `use std::collections::HashMap`.                                                            |
| 90    | Label                          | A lifetime labeling a for, while, or loop.                                                                     |
| 91    | Lifetime                       | A Rust lifetime: `'a`.                                                                                         |
| 92    | LifetimeParam                  | A lifetime definition: `'a: 'b + 'c + 'd`.                                                                     |
| 93    | LitBool                        | A boolean literal: `true or false`.                                                                            |
| 94    | LitByte                        | A byte literal: `b'f'`.                                                                                        |
| 95    | LitByteStr                     | A byte string literal: `b"foo"`.                                                                               |
| 96    | LitCStr                        | A null-terminated C-string literal: `c"foo"`.                                                                  |
| 97    | LitChar                        | A character literal: `'a'`.                                                                                    |
| 98    | LitFloat                       | A floating point literal: `1f64 or 1.0e10f64`.                                                                 |
| 99    | LitInt                         | An integer literal: `1 or 1u16`.                                                                               |
| 100   | LitStr                         | A UTF-8 string literal: `"foo"`.                                                                               |
| 101   | Local                          | A local let binding: `let x: u64 = s.parse()?`.                                                                |
| 102   | LocalInit                      | The expression assigned in a local let binding, including optional diverging else block.                       |
| 103   | Macro                          | A macro invocation: `println!("{}!", mac)`.                                                                    |
| 104   | MetaList                       | A structured list within an attribute, like `derive(Copy, Clone)`.                                             |
| 105   | MetaNameValue                  | A name-value pair within an attribute, like `feature = "nightly"`.                                             |
| 106   | ParenthesizedGenericArguments  | Arguments of a function path segment: the (A, B) -> C in `Fn(A, B) -> C`.                                      |
| 133   | PatConst                       | A pattern that contains a constant.                                                                            |
| 134   | PatIdent                       | A pattern that matches an identifier or wildcard: `mut var @ pat`.                                             |
| 135   | PatLit                         | A pattern that matches a literal value.                                                                        |
| 136   | PatMacro                       | A pattern that comes from an inline macro.                                                                     |
| 137   | PatOr                          | A pattern that matches any one of a list of patterns.                                                          |
| 138   | PatParen                       | A pattern enclosed in parentheses.                                                                             |
| 139   | PatPath                        | A pattern that matches a path to a constant.                                                                   |
| 140   | PatRange                       | A pattern that matches a range of values.                                                                      |
| 141   | PatReference                   | A pattern that matches a reference.                                                                            |
| 142   | PatRest                        | A pattern that matches the rest pattern: `..`.                                                                 |
| 143   | PatSlice                       | A pattern that matches a slice of values.                                                                      |
| 144   | PatStruct                      | A pattern that matches a struct.                                                                               |
| 145   | PatTuple                       | A pattern that matches a tuple.                                                                                |
| 146   | PatTupleStruct                 | A pattern that matches a tuple struct.                                                                         |
| 147   | PatType                        | A pattern that matches a type.                                                                                 |
| 148   | PatWild                        | A wildcard pattern: `_`.                                                                                       |
| 149   | Path                           | A path like `std::mem::replace`, possibly containing generic parameters and a self-type.                       |
| 150   | PathSegment                    | A segment of a path: `std`, `std::mem`, `std::mem::replace`.                                                   |
| 151   | PreciseCapture                 | Specifies precise capture behavior for closures.                                                               |
| 152   | PredicateLifetime              | A lifetime predicate in a where clause.                                                                        |
| 153   | PredicateType                  | A type predicate in a where clause.                                                                            |
| 154   | QSelf                          | The portion of a path before the `::`, if the path is qualified.                                               |
| 155   | Receiver                       | The self argument of an associated method: `&self` or `&mut self`.                                             |
| 156   | Signature                      | A function signature in a trait or impl block.                                                                 |
| 157   | StmtMacro                      | A macro invocation as a statement: `println!("Hello, world!")`.                                                |
| 158   | TraitBound                     | A trait bound on a type parameter or associated type.                                                          |
| 159   | TraitItemConst                 | An associated constant in a trait.                                                                             |
| 160   | TraitItemFn                    | An associated function in a trait.                                                                             |
| 161   | TraitItemMacro                 | A macro invocation in a trait.                                                                                 |
| 162   | TraitItemType                  | An associated type in a trait.                                                                                 |
| 163   | TurboFish                      | A turbo-fish, e.g., `collect::<Vec<_>>()`.                                                                     |
| 164   | TypeArray                      | An array type: `[T; n]`.                                                                                       |
| 165   | TypeBareFn                     | A bare function type: `fn(usize) -> bool`.                                                                     |
| 166   | TypeGenerics                   | A generic type parameter in a type definition.                                                                 |
| 167   | TypeGroup                      | A group of types.                                                                                              |
| 168   | TypeImplTrait                  | An `impl Trait` type in return position.                                                                       |
| 169   | TypeInfer                      | An inferred type: `_`.                                                                                         |
| 170   | TypeMacro                      | A macro in the type position.                                                                                  |
| 171   | TypeNever                      | The never type: !.                                                                                             |
| 172   | TypeParam                      | A generic type parameter: T: Into<String>.                                                                     |
| 173   | TypeParen                      | A parenthesized type equivalent to the inner type.                                                             |
| 174   | TypePath                       | A path like std::slice::Iter, optionally qualified with a self-type as in <Vec<T> as SomeTrait>::Associated.   |
| 175   | TypePtr                        | A raw pointer type: const T or \*mut T.                                                                        |
| 176   | TypeReference                  | A reference type: &'a Tor &'a mut T.                                                                           |
| 177   | TypeSlice                      | A dynamically sized slice type: [T].                                                                           |
| 178   | TypeTraitObject                | A trait object type dyn Bound1 Bound2 + Bound3 where Bound is a trait or a lifetime.                           |
| 179   | TypeTuple                      | A tuple type: (A, B, C, String).                                                                               |
| 180   | UseGlob                        | A glob import in a use item: \*.                                                                               |
| 181   | UseGroup                       | A braced group of imports in a use item: {A, B, C}.                                                            |
| 182   | UseName                        | An identifier imported by a use item: HashMap.                                                                 |
| 183   | UsePath                        | A path prefix of imports in a use item: std::..                                                                |
| 184   | UseRename                      | An renamed identifier imported by a use item: HashMap as Map.                                                  |
| 185   | Variadic                       | The variadic argument of a foreign function.                                                                   |
| 186   | Variant                        | An enum variant.                                                                                               |
| 187   | VisRestricted                  | A visibility level restricted to some path: pub (self) or pub (super) or pub (crate) or pub (in some::module). |
| 188   | WhereClause                    | A where clause in a definition: where T: Deserialize<'de>, D: 'static.                                         |

| STT | Tên nút           | Mô tả                                                                                                                                                           |
| --- | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | META_DATA         | Nút này chứa siêu dữ liệu (metadata) của đồ thị. Một đồ thị CPG phải có và chỉ có duy nhất một nút META_DATA.                                                   |
| 2   | FILE              | Nút biểu diễn một tệp mã nguồn. Với mỗi tệp tin trong mã nguồn, đồ thị sẽ có chính xác một nút FILE để biểu diễn tệp mã nguồn đó.                               |
| 3   | NAMESPACE         | Nút này biểu diễn một không gian tên (namespace) hoặc một gói (package), đối với Go, nút này biểu diễn các gói trong mã nguồn.                                  |
| 4   | NAMESPACE_BLOCK   | Nút này biểu diễn một tham chiếu đến không gian tên (namespace) tương ứng. Nó chứa các khối mã nguồn được định nghĩa dưới không gian tên (namespace) tương ứng. |
| 5   | METHOD            | Biểu diễn các hàm, phương thức hoặc biểu thức lambda.                                                                                                           |
| 6   | PARAMETER_IN      | Nút đại diện cho một tham số đầu vào của hàm.                                                                                                                   |
| 7   | PARAMETER_OUT     | Nút đại diện cho một tham số đầu ra của hàm.                                                                                                                    |
| 8   | METHOD_RETURN     | Nút này biểu diễn kiểu trả về của một hàm.                                                                                                                      |
| 9   | MEMBER            | Biểu diễn thuộc tính của một kiểu cấu trúc (struct).                                                                                                            |
| 10  | TYPE              | Nút đại diện cho một thể hiện (instance) của một kiểu dữ liệu.                                                                                                  |
| 11  | TYPE_ARGUMENT     | Biểu diễn đối số của một kiểu dữ liệu, có thể hình dung giống như các kiểu dữ liệu generic trong JAVA.                                                          |
| 12  | TYPE_DECL         | Biểu diễn một khai báo kiểu dữ liệu ví dụ như khai báo một kiểu cấu trúc (struct) hay khai báo một giao diện (interface).                                       |
| 13  | BLOCK             | Biểu diễn một khối mã nguồn.                                                                                                                                    |
| 14  | CALL              | Biểu diễn một lời gọi hàm.                                                                                                                                      |
| 15  | CONTROL_STRUCTURE | Biểu diễn một cấu trúc điều khiển ví dụ như câu lệnh if else, vòng lặp for, cấu trúc switch case.                                                               |
| 16  | IDENTIFIER        | Nút định danh biểu diễn tham chiếu đến một biến.                                                                                                                |
| 17  | JUMP_LABEL        | Biểu diễn các cấu trúc nhảy như BREAK, CONTINUE, GOTO.                                                                                                          |
| 18  | LITERAL           | Biểu diễn một hằng số như số nguyên hoặc chuỗi.                                                                                                                 |
| 19  | LOCAL             | Biểu diễn một biến cục bộ.                                                                                                                                      |
| 20  | METHOD_REF        | Biểu diễn một tham chiếu đến hàm khi hàm đó được dùng làm tham số cho một lời gọi.                                                                              |
| 21  | MODIFIER          | Biểu diễn một bộ chỉnh sửa (modifier) như static, public hay private.                                                                                           |
| 22  | RETURN            | Biểu diễn một chỉ thị trả về (return instruction).                                                                                                              |
| 23  | TYPE_REF          | Biểu diễn tham chiếu đến một kiểu dữ liệu.                                                                                                                      |

| STT | Tên nút        | Mô tả                                                                                                                                                                                                        |
| --- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | SOURCE_FILE    | Quan hệ biểu diễn một nút là tệp gốc của một nút khác. Quan hệ cha con (biểu diễn quan hệ trong cây cú pháp mã nguồn (AST)).                                                                                 |
| 2   | AST            | Cây cú pháp trừu tượng (Abstract Syntax Tree).                                                                                                                                                               |
| 3   | CALL           | Quan hệ gọi, dùng để biểu diễn quan hệ giữa hàm/phương thức với nút gọi hàm/phương thức đó.                                                                                                                  |
| 4   | CONTAINS       | Quan hệ bao gồm.                                                                                                                                                                                             |
| 5   | CONDITION      | Quan hệ điều kiện, dùng để biểu diễn quan hệ giữa khối điều khiển như if else, switch hay for với biểu thức điều kiện của chúng.                                                                             |
| 6   | ARGUMENT       | Quan hệ đối số kết nối các điểm gọi (kiểu nút CALL) với các đối số của chúng, cũng như các nút RETURN với các biểu thức trả về.                                                                              |
| 7   | RECEIVER       | Quan hệ kết nối các điểm gọi (CALL) tới đối số nhận (receiver argument) của chúng. Một đối số nhận là một đối tượng mà phương thức đó thuộc về (có thể hiểu đối số nhận ở đây là con trỏ 'this' trong Java). |
| 8   | CFG            | Quan hệ này biểu diễn luồng điều khiển từ nút nguồn đến nút đích.                                                                                                                                            |
| 9   | DOMINATE       | Quan hệ biểu diễn tính kiểm soát (dominate) ngay lập tức từ nút nguồn đến nút đích.                                                                                                                          |
| 10  | POST_DOMINATE  | Quan hệ biểu diễn nút nguồn kiểm soát (dominate) ngay lập tức sau nút đích.                                                                                                                                  |
| 11  | CDG            | Quan hệ biểu diễn nút đích phụ thuộc điều khiển vào nút nguồn.                                                                                                                                               |
| 12  | REACHING_DEF   | Quan hệ biểu diễn một biến được tạo ra từ nút nguồn và không bị gán lại giá trị trên đường đi tới nút đích.                                                                                                  |
| 13  | CONTAINS       | Quan hệ này kết nối một nút tới hàm/phương thức chứa nó.                                                                                                                                                     |
| 14  | EVAL_TYPE      | Quan hệ kết nối một nút tới nút kiểu dữ liệu của nút đó.                                                                                                                                                     |
| 15  | PARAMETER_LINK | Quan hệ kết nối một nút tham số đầu vào với nút tham số đầu ra tương ứng của hàm/phương thức đó.                                                                                                             |

# Prompt

1. seperate each sentences into 1 line

# Representing LLVM-IR in a Code Property Graph

# Modeling and Discovering Vulnerabilities with Code Property Graphs

# A Closer Look at the Security Risks in the Rust Ecosystem

# YUGA: Automatically Detecting Lifetime Annotation Bugs in the Rust Language

# RUDRA: Finding Memory Safety Bugs in Rust at the Ecosystem Scale

# RustBelt: Securing the Foundations of the Rust Programming Language

# Stacked Borrows: An Aliasing Model for Rust (Miri)

# Rust for Embedded Systems: Current State and Open Problems (Extended Report)

# Bringing Rust to Safety-Critical Systems in Space
