# 编程概念

本篇主要讲述在 Rust 中如何使用变量，运行使用函数，以及流程控制

### 变量

声明变量的方式有 2 种，一种是 let,另一种是 const。

```rust
let name_1 = "Glay"
const NAME_2 = "GLAY"
```

两者声明的变量都是不可变，举一个可以重新赋值的 🌰

```rust
fn main() {
    let mut a = 123;

    a = 222;

    println!("a is {}", a);
}
```

除此之外，还有 2 点不同：

1. 在 Rust 中，`let`和`const`的区别在于它们的求值时间点和赋值。`const`是在编译时求值，而`let`是在编译时绑定，求值时间点取决于赋值语句右侧值的类型。常量表达式在编译时求值，普通表达式在运行时求值。

2. `const`仅接受常量表达式，而`let`既可以接受常量表达式，也能够接受运行时求值的普通表达式。

```rust
// ❌ 示例
const B: i32 = 5645;
// cannot assign to this expression
B = 777;

println!("B is {}", B);

fn reurn_num () -> i32 {
    return 66
}
// cannot call non-const fn `reurn_num` in constants
// calls in constants are limited to constant functions, tuple structs and tuple variants
const B: i32 = reurn_num();

// ✅ 示例
const B: i32 = 5645 * 44;

println!("B is {}", B);
```
