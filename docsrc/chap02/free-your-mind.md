# Free Your Mind: Interactive Programming（放开思想：交互式编程）

When you start Lisp in a Box, you should see a buffer containing a prompt that looks like this:

当启动 Lisp-in-a-Box 时，应该可以看到一个带有类似下面提示符的缓冲区：

```
CL-USER> 10
```

This is the Lisp prompt. Like a Unix or DOS shell prompt, the Lisp
prompt is a place where you can type expressions that will cause
things to happen. However, instead of reading and interpreting a line
of shell commands, Lisp reads Lisp expressions, evaluates them
according to the rules of Lisp, and prints the result. Then it does it
again with the next expression you type. That endless cycle of
reading, evaluating, and printing is why it's called the
read-eval-print loop, or REPL for short. It's also referred to as the
top-level, the top-level listener, or the Lisp listener.

这是 Lisp 的提示符。就像 Unix 或 DOS shell 提示符那样，在 Lisp
提示符的位置上输入表达式可以产生一定的结果。尽管如此，Lisp 读取的是
Lisp 表达式而非一行 shell 命令，按照 Lisp
的规则来对它求值，然后打印结果。接着它再继续处理你输入的下一个表达式。正是由于这种无休止的读取、求值和打印的周期变化，因此它被称为读-求值-打印循环（read-eval-print
loop），简称 REPL。它也被称为顶层（top-level）、顶层监听器（top-level
listener）或 Lisp 监听器。

From within the environment provided by the REPL, you can define and
redefine program elements such as variables, functions, classes, and
methods; evaluate any Lisp expression; load files containing Lisp
source code or compiled code; compile whole files or individual
functions; enter the debugger; step through code; and inspect the
state of individual Lisp objects.

借助 REPL 提供的环境就可以定义或重定义诸如变量、函数、类和方法等程序要素，求值任何
Lisp 表达式，加载含有 Lisp
源代码或编译后代码的文件，编译整个文件或者单独的函数，进入调试器，单步调试代码，以及检查个别
Lisp 对象的状态。

All those facilities are built into the language, accessible via
functions defined in the language standard. If you had to, you could
build a pretty reasonable programming environment out of just the REPL
and any text editor that knows how to properly indent Lisp code. But
for the true Lisp programming experience, you need an environment,
such as SLIME, that lets you interact with Lisp both via the REPL and
while editing source files. For instance, you don't want to have to
cut and paste a function definition from a source file to the REPL or
have to load a whole file just because you changed one function; your
Lisp environment should let us evaluate or compile both individual
expressions and whole files directly from your editor.

所有这些机制都是语言内置的，可以通过语言标准所定义的函数来访问。如果有必要，你只需使用
REPL 和一个知道如何正确缩进 Lisp
代码的文本编辑器，就可以构建出一个相当合理的编程环境来。但如果追求真正的
Lisp 编程体验，则需要一个像 SLIME 这样的环境，它可以同时通过
REPL 和编辑源文件时与 Lisp 进行交互。
例如，没有必要把一个函数定义从源文件里复制并粘贴到 REPL
里，也不必因为改变了一个函数就把整个文件重新加载。Lisp
环境应该允许编译单独的表达式和直接来自编辑器的整个文件或对其求值。
