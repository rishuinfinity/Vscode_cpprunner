# Vscode_cpprunner
Run cpp files with input file and output file with  this shortcut.

# Pre-requisites
* Install Vs-code
* Install g++

# Steps
* Press Ctrl+Shift+P on VScode
* Then type keyboard and select "Open Keyboard Shortcuts(JSON)"
* Add the following in the []
  ```
  {
        "key": "ctrl+enter",
        "command": "workbench.action.terminal.sendSequence",
        "args": {
          "text": "g++ -o ~/.cache/g++/files/temp.out $(pwd)/${fileBasename}; ~/.cache/g++/files/temp.out < $(pwd)/input.txt > $(pwd)/output.txt;\u000D"
        }
  }
  ```
* You can modify the key to change the shortcut, by default it is ctrl+enter.

# How to run
* Make sure you have a file named input.txt in the same directory where your cpp file is.
* When you want to run, save the Cpp file and while you are in the same window, press Ctrl+enter (or any other shortcut that you have set).
* The output will be saved in an output file.
