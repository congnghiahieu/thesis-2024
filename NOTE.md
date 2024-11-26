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

# A Language-Independent Analysis Platform for Source Code

# Modeling and Discovering Vulnerabilities with Code Property Graphs

# A Closer Look at the Security Risks in the Rust Ecosystem

- We find that memory safety and concurrency issues account for nearly two thirds of the vulnerabilities in the Rust ecosystem

## RQ1: What are the characteristics of the vulnerabilities in the Rust ecosystem?

- Our study identified 17 types of vulnerabilities disclosed in the Rust ecosystem, among which memory safety and concurrency issues account for two-thirds of the categorized vulnerabilities and demonstrate the fastest growth rates over time.

## RQ2: What are the characteristics of the vulnerable packages in the Rust ecosystem?

- The memory management package category has the greatest number of vulnerabilities per package among different Rust package categories, and tends to have more memory access, memory management, and synchronization vulnerabilities as compared to other package categories

- In the vulnerable packages, vulnerable code has statistically significantly higher ratios of unsafe functions and unsafe blocks compared to complete code, implying the potential higher security risks in unsafe functions and unsafe blocks.

## 3.3 Characterizing Vulnerabilities, Vulnerable Packages, and Fixes

- The vulnerabilities from the four sources use two classification schemes, i.e., Common Weakness Enumeration (CWE) and RustSec categorization.

- As shown in Table 1, we identified 17 vulnerability types in our dataset

| Vulnerability Type        | RustSec Category     |
| ------------------------- | -------------------- |
| Memory Access             | memory-exposure      |
| Memory Management         | memory-corruption    |
| Synchronization           | thread-safety        |
| Tainted Input             | format-injection     |
| Resource Management       | denial-of-service    |
| Exception Management      | -                    |
| Cryptography              | cryptography         |
| Risky Values              | -                    |
| Path Resolution           | file-disclosure      |
| Information Leak          | -                    |
| Privilege                 | privilege-escalation |
| Predictability            | -                    |
| Authentication            | -                    |
| API                       | -                    |
| Access Control            | -                    |
| Failure to Release Memory | -                    |
| Other                     | code-execution       |

## 4 RESULTS

### 4.1 RQ1: Vulnerabilities in the Rust Ecosystem

- Types of vulnerabilities. We collected a total of 433 unique vulnerabilities in the Rust ecosystem, out of which 73 have not been categorized, leaving 360 vulnerabilities that are categorized with a median of 1 vulnerability type (min: 1, max: 4, mean: 1.65, std: 0.76). Table 3 presents the overall distribution of vulnerabilities across 17 vulnerability types. Memory safety and concurrency issues account for 63.6% of the 360 categorized vulnerabilities. Memory safety issues involve memory access (39.17%) and memory management (40.00%) vulnerability types, accounting for 59.7% of the categorized vulnerabilities. The memory access vulnerabilities usually arise from buffer or pointer access problems, e.g., buffer overflow, use after free, and null pointer deference. We take the RUSTSEC-2021-0128 in the rusqlite package as an example of memory access vulnerability. In the vulnerable code of the rusqlite package affected by RUSTSEC-2021-0128, the lifetime bounds on several closure-accepting functions are so loose that allow the access to dropped objects on the stack thus cause use after free error. The memory management vulnerabilities are due to problems in memory allocation or deallocation, e.g., double free. RUSTSEC-2021-0033 in the stack_dst package is an example of memory management vulnerabilities. Specifically, the push_cloned function in the vulnerable code of stack_dst package deallocates uninitialized memory thus cause double free error. Concurrency issues involve synchronization vulnerabilities, which rank the third in the frequency of occurrence across different types of vulnerabilities (20.56%). The Synchronization vulnerabilities occur when multiple processes or threads share resources, including race condition and misuse of locks. For instance, the unsafe Send trait implementation in the atom package involved in RUSTSEC-2020-0044 causes data race error.

- Summary for RQ1: The top three vulnerability types in the Rust ecosystem are memory access, memory management, and synchronization, accounting for 63.6% of categorized vulnerabilities and exhibiting the fastest growth rates

### 4.3 RQ3: Vulnerability Fixes in the Rust Ecosystem

- Observation 1: Developers tend to add safe functions, or add lines in safe functions to
  fix vulnerable safe functions.

- Observation 2: Developers tend to remove unsafe blocks to fix vulnerable unsafe blocks.

- Observation 3: Developers tend to modify unsafe trait implementations to fix vulnerable
  unsafe functions.

# YUGA: Automatically Detecting Lifetime Annotation Bugs in the Rust Language

## 3.2 Algorithm Design

- Step-I. YUGA extracts lifetimes from each type of a function signature.
- Step-II. Next, YUGA uses these lifetimes to check for the LA bug patterns identified in Section 3.1 and marks potential buggy functions.
- Step-III. The potential buggy functions are then sent to an alias analyzer to check whether values are actually transferred between the locations with LAs
- Step-IV. Finally, YUGA filters out some common patterns of false positives that arise due to intra-procedural alias analysis.

## 4.1 Implementation

- When Rust code is compiled, it goes through several intermediate representations (IRs), two of which are the High level IR (HIR) and the Mid-level IR (MIR). The HIR is a tree representation of the program that is similar to an Abstract Syntax Tree (AST). The MIR represents each function as a control-flow graph of basic blocks, with each basic block consisting of a number of statements. MIR boils the different kind of statements occurring in a program down to a core set of statement types like assignments, memory allocation, and memory de-allocation. We use a hybrid approach that combines information from the HIR and the MIR. We use the HIR to get struct definitions and function signatures, and use the MIR to perform alias analysis

## 5.1 RQ1: Effectiveness of our Tool

## 5.3 RQ3: Comparison with existing tools

- Rudra is a static analysis tool that identifies three types of potential memory and thread safety violations - panic safety, higher order safety invariant, and Send/Sync variance. It is not explicitly designed to detect LA bugs;

- MirChecker is a static analysis tool for the Rust MIR based on the theory of Abstract Interpretation. It forms a control flow graph (CFG) of the program, defines a transfer function for each value and statement, and propagates these values across the CFG to reach a fixed point. It then uses these values to detect potential vulnerabilities in Rust code.

- Miri is an interpreter for the Rust MIR. It emulates the execution of each line of code using a virtual address space, and can detect memory leaks, out of bounds accesses, and other potential vulnerabilities. This is a dynamic tool, and deals with actual vulnerabilities that arise when Rust code is run. In contrast, YUGA deals with potential vulnerabilities that could arise when a function is called in a certain context. So we expect Miri to detect LA bugs if and only if the exploit code is also provided

## 7 RELATED WORK

- Dynamic testing of Rust code: Miri [16] is an interpreter to detect invalid memory accesses or memory leaks (see Section 5.3). Stacked Borrows[26] (incorporated into Miri) develops a “stack” model to reason about borrows without explicitly using lifetimes.

- Static analysis for detecting bugs in Rust: MirChecker [13] and SafeDrop [14] are static analyzers on the Rust MIR that detect certain memory safety errors. However, much like dynamic approaches, these approaches tend to have high false negatives. Rudra [12] identifies three categories of bugs arising from unsafe code, and scans the entire Rust crate ecosystem for these bug patterns. Rudra is the closest work to ours in the sense that it uses static analysis to identify potential memory safety violations. However, Rudra can handle only three specific kinds of errors, and cannot detect memory safety bugs caused by incorrect lifetime annotations

- There have also been attempts to model the semantics of unsafe Rust. RustBelt [34] develops a comprehensive formal semantics based on lifetimes for a realistic subset of Rust including unsafe code. However, this cannot scale to larger codebases and crates. Verifying the safety of a given library with RustBelt involves writing proofs with the Coq proof assistant [35], which requires considerable expertise and effort. In contrast, our approach aims to be a lightweight automatic error detector that can aid developers.

# RUDRA: Finding Memory Safety Bugs in Rust at the Ecosystem Scale

## 2.3 Defining Memory Safety Bugs in Rust

- Các definition, example là các pattern, luật

## 4 Design

- Generic type awareness. RUDRA should be able to reason about generic types without knowing the concrete forms of their type parameters. This means that low-level analysis (e.g., using LLVM IR) is not an option. Low-level representations only contain a specific instantiation of generic code, and Rust’s high-level abstractions such as trait variance do not exist at these levels. Instead, RUDRA implements algorithms by combining two internal IRs of the Rust compiler, namely, HIR and MIR.

- Scalability. As our primary goal is to check all the packages in the Rust package registry, it is critical to strike a balance between the precision of analysis and the execution time—expensive whole-program analyses and dynamic analyses like fuzzing are not feasible options for RUDRA. In addition, RUDRA aims to be a push-button solution that requires no manual annotation and effort from the original package developers.

## 4.1 Hybrid Analysis with HIR and MIR

## 6.2 Comparison with Other Approaches

## 8 Related work

# Stacked Borrows: An Aliasing Model for Rust (Miri)

# RustBelt: Securing the Foundations of the Rust Programming Language

# Bringing Rust to Safety-Critical Systems in Space

- Rust was first introduced in 2006 by the Mozilla Foundation with its version 1.0 release announced in 2015

# Rust for Embedded Systems: Current State and Open Problems (Extended Report)

- It is important to use memory-safe languages to prevent such vulnerabilities. Furthermore, recently, the White House released a report [143] requiring future software to be developed in memory-safe languages. Traditional memory safe languages, such as Java, have high overhead and are not suitable for embedded systems. Rust [125] is a memory-safe language that is shown to have comparable performance as native code. Furthermore, Rust can easily interoperate with existing unsafe codebases [63], enabling incremental adoption. Rust team has a special focus on embedded systems [116], and several works [76, 77] demonstrate the feasibility of engineering a complete embedded software stack in Rust. Furthermore, Rust popularity is rising [103], and it is now adopted in Linux kernel [81] and Android [111].
