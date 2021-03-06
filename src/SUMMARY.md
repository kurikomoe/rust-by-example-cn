# Summary

[简介](index.md)

- [Hello World](hello.md)
    - [注释](hello/comment.md)
    - [格式化输出](hello/print.md)
        - [调试](hello/print/print_debug.md)
        - [显示](hello/print/print_display.md)
            - [测试实例：List](hello/print/print_display/testcase_list.md)
        - [格式化](hello/print/fmt.md)

- [原生类型](primitives.md)
    - [数据和运算符](primitives/literals.md)
    - [元组](primitives/tuples.md)
    - [数组和 slice 类型](primitives/array.md)

- [自定义类型](custom_types.md)
    - [结构体](custom_types/structs.md)
    - [枚举](custom_types/enum.md)
        - [使用 use](custom_types/enum/enum_use.md)
        - [C 风格用法](custom_types/enum/c_like.md)
        - [测试实例：链表](custom_types/enum/testcase_linked_list.md)
    - [常量](custom_types/constants.md)

- [变量绑定](variable_bindings.md)
    - [可变变量](variable_bindings/mut.md)
    - [作用域和隐藏](variable_bindings/scope.md)
    - [变量先声明](variable_bindings/declare.md)

- [类型转换](cast.md)
    - [字面量](cast/literals.md)
    - [类型推导](cast/inference.md)
    - [别名](cast/alias.md)

- [表达式](expression.md)

- [流程控制](flow_control.md)
    - [if/else](flow_control/if_else.md)
    - [loop 循环](flow_control/loop.md)
        - [嵌套循环和标签](flow_control/loop/nested.md)
        - [从 loop 循环返回](flow_control/loop/return.md)
    - [while 循环](flow_control/while.md)
    - [for 循环和区间](flow_control/for.md)
    - [match 匹配](flow_control/match.md)
        - [解构](flow_control/match/destructuring.md)
            - [元组](flow_control/match/destructuring/destructure_tuple.md)
            - [枚举](flow_control/match/destructuring/destructure_enum.md)
            - [指针和引用](flow_control/match/destructuring/destructure_pointers.md)
            - [结构体](flow_control/match/destructuring/destructure_structures.md)
        - [守卫](flow_control/match/guard.md)
        - [绑定](flow_control/match/binding.md)
    - [if let](flow_control/if_let.md)
    - [while let](flow_control/while_let.md)

- [函数](fn.md)
    - [方法](fn/methods.md)
    - [闭包](fn/closures.md)
        - [捕获](fn/closures/capture.md)
        - [作为输入参量](fn/closures/input_parameters.md)
        - [类型匿名](fn/closures/anonymity.md)
        - [输入函数](fn/closures/input_functions.md)
        - [作为输出参量](fn/closures/output_parameters.md)
        - [`std` 中的例子](fn/closures/closure_examples.md)
            - [Iterator::any](fn/closures/closure_examples/iter_any.md)
            - [Iterator::find](fn/closures/closure_examples/iter_find.md)
    - [高阶函数](fn/hof.md)

- [模块](mod.md)
    - [可见性](mod/visibility.md)
    - [结构体的可见性](mod/struct_visibility.md)
    - [`use` 声明](mod/use.md)
    - [`super` 和 `self`](mod/super.md)
    - [文件分层](mod/split.md)

- [crate](crates.md)
    - [库](crates/lib.md)
    - [`extern crate`](crates/link.md)

- [属性](attribute.md)
    - [死代码 `dead_code`](attribute/unused.md)
    - [`crate`](attribute/crate.md)
    - [`cfg`](attribute/cfg.md)
        - [自定义条件](attribute/cfg/custom.md)

- [泛型](generics.md)
    - [函数](generics/gen_fn.md)
    - [实现](generics/impl.md)
    - [特性 trait](generics/gen_trait.md)
    - [限定](generics/bounds.md)
        - [测试实例：空限定](generics/bounds/testcase_empty.md)
    - [多重限定](generics/multi_bounds.md)
    - [where 从句](generics/where.md)
    - [关联项](generics/assoc_items.md)
        - [存在问题](generics/assoc_items/the_problem.md)
        - [关联类型](generics/assoc_items/types.md)
    - [虚位类型参量](generics/phantom.md)
        - [测试实例：单位阐明](generics/phantom/testcase_units.md)

- [作用域规则](scope.md)
    - [RAII](scope/raii.md)
    - [所有权和移动](scope/move.md)
        - [可变性](scope/move/mut.md)
    - [借用](scope/borrow.md)
        - [可变性](scope/borrow/mut.md)
        - [冻结](scope/borrow/freeze.md)
        - [别名使用](scope/borrow/alias.md)
        - [ref 模式](scope/borrow/ref.md)
    - [生命周期](scope/lifetime.md)
        - [显示标注](scope/lifetime/explicit.md)
        - [函数](scope/lifetime/fn.md)
        - [方法](scope/lifetime/methods.md)
        - [结构体](scope/lifetime/struct.md)
        - [限定](scope/lifetime/lifetime_bounds.md)
        - [强制转换](scope/lifetime/lifetime_coercion.md)
        - [静态](scope/lifetime/static_lifetime.md)
        - [省略](scope/lifetime/elision.md)

- [特性 trait](trait.md)
    - [派生](trait/derive.md)
    - [运算符重载](trait/ops.md)
    - [Drop](trait/drop.md)
    - [Iterators](trait/iter.md)
    - [Clone](trait/clone.md)

- [使用 `macro_rules!` 来创建宏](macros.md)
    - [指示符](macros/designators.md)
    - [重载](macros/overload.md)
    - [重复](macros/repeat.md)
    - [DRY (不写重复代码)](macros/dry.md)

- [错误处理](error.md)
    - [`panic`](error/panic.md)
    - [`Option` & `unwrap`](error/option_unwrap.md)
        - [组合算子：`map`](error/option_unwrap/map.md)
        - [组合算子：`and_then`](error/option_unwrap/and_then.md)
    - [结果 `Result`](error/result.md)
        - [关于 `Result` 的 `map`](error/result/result_map.md)
        - [给 `Result` 起别名](error/result/result_alias.md)
    - [各种错误类型](error/multiple_error_types.md)
        - [提前返回](error/multiple_error_types/early_returns.md)
        - [介绍 `try!`](error/multiple_error_types/enter_try.md)
    - [定义一个错误类型](error/define_error_type.md)
    - [try!` 的其他用法](error/reenter_try.md)
    - [使用 `Box` 处理错误](error/boxing_errors.md)

- [标准库类型](std.md)
    - [Box, 以及栈和堆](std/box.md)
    - [动态数组 vector](std/vec.md)
    - [字符串 String](std/str.md)
    - [选项 `Option`](std/option.md)
    - [结果 `Result`](std/result.md)
        - [`?`](std/result/question_mark.md)
    - [`panic!`](std/panic.md)
    - [散列表 HashMap](std/hash.md)
        - [更改或自定义关键字类型](std/hash/alt_key_types.md)
        - [散列集 HashSet](std/hash/hashset.md)

- [标准库更多介绍](std_misc.md)
    - [线程](std_misc/threads.md)
    - [通道](std_misc/channels.md)
    - [路径 Path](std_misc/path.md)
    - [文件输入输出 I/O](std_misc/file.md)
        - [打开文件 `open`](std_misc/file/open.md)
        - [创建文件 `create`](std_misc/file/create.md)
    - [子进程](std_misc/process.md)
        - [管道](std_misc/process/pipe.md)
        - [等待 Wait](std_misc/process/wait.md)
    - [文件系统操作](std_misc/fs.md)
    - [程序参数](std_misc/arg.md)
        - [参数分析](std_misc/arg/matching.md)
    - [外部语言函数接口](std_misc/ffi.md)

- [补充](meta.md)
    - [文档](meta/doc.md)
    - [测试](meta/test.md)

- [不安全操作](unsafe.md)
