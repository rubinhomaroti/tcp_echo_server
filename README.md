# TCP Echo Server

Exercise from chapter 2 **"TCP: Exploring the Basics"** from ["Network Programming in Elixir and Erlang"](https://pragprog.com/titles/alnpee/network-programming-in-elixir-and-erlang/) book

## How to run?

1. Start the server: `mix run --no-halt`
2. Send a message in another terminal: `echo "Hello world\nThis is a TCP server in action!" | nc localhost 4000`
3. Check the logs in server output
```
➜  tcp_echo_server git:(main) ✗ mix run --no-halt

20:42:32.788 [info] Started TCP server on port 4000

20:42:40.090 [debug] ### Data received: 'Hello world'

20:42:40.090 [debug] ### Data received: 'This is a TCP server in action'
```