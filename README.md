# Introduction

If you're running a program in the terminal on a remote Ubuntu server and you want to exit the terminal without stopping the program, you can do so by using a terminal multiplexer [tmux](https://github.com/tmux/tmux/wiki).

This tool allow you to create virtual terminal sessions that persist even after you disconnect from the remote server. Follow the steps below to use tmux:

# Step by Step

1. Install tmux

   ```bash
   sudo apt install tmux
   ```

2. Start a new tmux session

   ```bash
   tmux
   ```

3. Detach from the tmux session
   To detach from the tmux session without stopping your program, _*press Ctrl+b then press d*_. This will return you to the regular terminal session, but your program will continue running inside the tmux session.

4. Exit the terminal then reattach the session
   You can now exit the terminal without stopping your program. When you want to reattach to the tmux session later, you can log back into your Ubuntu server and run:

   ```bash
   tmux attach
   ```
