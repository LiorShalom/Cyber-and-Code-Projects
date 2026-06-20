# TCP Chat Server

A multi-user chat application built with Python sockets. It has two parts — a **server** that handles all connections and a **client** that people run to join the chat. Multiple users can sign up, log in, and message each other in real time.

## What's inside

| File | Role |
|------|------|
| `server.py` | Runs the chat server — accepts connections, manages accounts, broadcasts messages |
| `client.py` | What each user runs to connect, sign up / log in, and chat |
| `Multi-user chat server in Python.pdf` | Full written project review / documentation |

## Features

- **Accounts** — sign up with a name, username, and password; log in to reconnect
- **Multiple users at once** — the server uses `select` to handle many connections in a single thread
- **Live notifications** — everyone sees when a user connects or disconnects
- **Two network modes** — run on `localhost` to test on one machine, or on your local IPv4 to let others on the same network join
- **Colored terminal output** — via the `colorama` library
- **Clean shutdown** — type `shutdown` on the server to disconnect everyone safely; type `exit()` on a client to leave

## How to run

You need Python 3. The scripts auto-install `colorama` if it's missing.

**1. Start the server** (on one machine):
```bash
python3 server.py
```
Choose option `1` (localhost) for a solo test, or `2` (local IPv4) to let others connect. The server prints the HOST/IP and PORT to share.

**2. Start a client** (on each user's machine):
```bash
python3 client.py
```
Enter the server's HOST/IP and PORT when prompted, then sign up or log in.

## What I learned

- TCP socket programming (`socket`, bind/listen/accept)
- Handling many clients in one thread with `select`
- Running send/receive at the same time with `threading`
- Building a simple account + login system
- Encoding/decoding messages and a basic message protocol
