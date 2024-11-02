Hey! This is my NeoVim config based on NvChad V2.5. I’ve added some tweaks from ProgrammingRainbow (https://www.youtube.com/@ProgrammingRainbow) and set up the C/C++ debugger using CodeLLDB through nvim-dap.

Here’s how it works:
1. First, compile your program through the command line (you can do this directly in NeoVim).
2. Once compiled, you can debug your code with CodeLLDB using the shortcut keys (check them in the lua.dap file).

A few setup steps:
- In dap.lua, make sure to specify the folder location of your codelldb after "command =". You can use either an independently installed version or the one installed via Mason.
- If you’re using the version from Mason, find its path by running this command:

lua print(vim.fn.stdpath("data") .. "/mason/packages/codelldb/")

Happy coding and debugging!
