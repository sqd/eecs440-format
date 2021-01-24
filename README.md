# EECS 440 C++ Style Formatter
[Linux binary download](https://github.com/sqd/eecs440-format/releases/download/v0.0.1/clang-format-440)
#### Short usage: `./clang-format-440 --style=EECS440 -i file1.cpp file2.cpp`

#### - Why should I use this formatter instead of astyle or clang-format?
- clang-format: doesn't really work because of some bizzare styling choices of the stylesheet.
- astyle: mostly works (**doesn't support double space after semicolon, while this tool does**). However, with this tool, you can add on your favorite clang-format configs from your IDE, while astyle does not understand those.

#### - How?
- Modified clang-format from LLVM 11.0.0.

#### - Longer usage:
- Because this tool is modified from clang-format, you could do whatever you would clang-format.
- To apply EECS 440 style, use the option `--style="{BasedOnStyle: EECS440}"`. Alternatively, in your .clang-format config, use `BasedOnStyle: EECS440`
- All options of the original clang-format are kept. Some might not take effect while EECS 440 style is used.

#### - Help wanted
- Compile a Mac version! I don't have a Mac.
- Compile a Windows version! I might do it if I have time.

#### - Bugs?
- Create an issue.
