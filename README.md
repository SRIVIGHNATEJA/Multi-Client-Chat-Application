# 🧠 CN Project – Multi-Client Chat Application in C

> **Title:** `Multithreaded Chat Server-Client System using C and Socket Programming`

## 📌 About the Project

This is a **multi-client, real-time chat application** developed in **C**, as a part of the **Computer Networks Lab Project** at **Sreyas Institute of Engineering and Technology**. It combines core CN concepts like **TCP socket programming**, **client-server communication**, and **multithreading** via `pthread` to simulate a real-world terminal-based messaging system.

The application offers:

* Secure **user registration and login system**
* **Simultaneous multi-client connections** with isolated threads
* **Broadcast messaging** to all online users
* **Private messaging** to any specific user
* **Clean flow of user choices and actions** with complete input validation

## 🚀 Highlights of the Project's Significance

* ✅ **Practical Implementation** of CN topics using real system-level C code
* ✅ **Built from scratch** with design planning, socket API usage, and thread-safe communication
* ✅ Demonstrated on **multi-terminal VS Code** showing real-time chats between users
* ✅ Offers a **hands-on understanding** of server lifecycle, connection handling, and command-based message routing
* ✅ Designed for Linux/macOS terminals—**not a GUI simulation**, but a working terminal prototype

> 🔐 Unlike traditional projects, this system is unique in its design, logic flow, and login mechanics.

## 📁 Project Structure

```bash
📦 CN-Chat-Application
├── client.c             # Client-side implementation (registration/login, menus, message sending)
├── server.c             # Server-side implementation (threaded client handling, routing logic)
├── client               # Compiled client binary
├── server               # Compiled server binary
├── LICENSE              # Apache License 2.0
├── README.md            # This file
├── *.dSYM               # macOS debug folders (auto-generated, can ignore)
├── a.out                # Default compilation output (ignore)
```

---

## 🔄 Functional Flow (Execution Demo)

### 🔧 Compilation

```bash
$ gcc client.c -o client -lpthread
$ gcc server.c -o server -lpthread
```

### 🚦 Server Start

```bash
$ ./server
Server is running...
```

### 🧑‍💻 Client Terminals (Multiple)

```bash
$ ./client
Enter username:
```

Users can:

1. **Register** with a username and password
2. **Login** to chat
3. Send messages via:

   * `1. Broadcast` → All users
   * `2. Private message` → One specific user
4. `3. Logout` → Exit chat

---

## 🔍 Sample Chat Flow

* **User 1 (Teja):** Registers, logs in, sends broadcast message
* **User 2 (Ravi):** Registers, logs in, receives broadcast, sends private message
* **User 3 (Ram):** Logs in to receive all messages

All operations are real-time with thread-safe socket communication.

---

## 🛠️ Technologies Used

| Category       | Tools/Concepts                   |
| -------------- | -------------------------------- |
| Language       | C                                |
| Networking     | TCP, POSIX sockets               |
| Multithreading | pthread                          |
| System API     | unistd.h, arpa/inet.h            |
| Testing        | VS Code terminals (side-by-side) |
| Platform       | macOS/Linux                      |

---

## 🔐 License

Licensed under the [Apache License 2.0](./LICENSE)

## 🙌 Author & Credit

**Developed by:** *Sri Vighna Teja*
**Department:** AIML, Sreyas Institute of Engineering and Technology
**Semester:** 2nd Year CN Lab Project (Now in Final Year)

---

💬 For demonstration and academic purposes only.
