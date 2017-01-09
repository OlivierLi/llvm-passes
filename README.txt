These are some llvm passes that I play around with.

## Trying them out

The easiest way to try out these passes is actually to simply use the facilities provided by the llvm repo itself.

## Steps:

1. [Get and build the llvm source code](http://llvm.org/docs/GettingStarted.html#getting-started-quickly-a-summary)
2. Replace `$LLVM_DIR/lib/Transforms/Hello/Hello.cpp` with one of these passes
3. Rebuild llvm.
4. Go to `$LLVM_DIR/build/`
5. Compile some code with your pass activated using `./bin/clang++ -Xclang -load -Xclang ../lib/LLVMHello.so MyCode.cpp`
6. That's it!
