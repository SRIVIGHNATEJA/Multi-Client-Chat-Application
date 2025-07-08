# 🧠 CN Project – Multi-Client Chat Application in C

> **Title:** `Multithreaded Chat Server-Client System using C and Socket Programming`

## 📌 About the Project

This is a **multi-client chat-based application** built using the **C programming language**, implemented as part of a semester project for the **Computer Networks** course at **Sreyas Institute of Engineering and Technology**. It demonstrates core networking concepts using **sockets**, **multi-threading**, and **POSIX APIs** on **Linux/macOS platforms**.

The system allows:

* User **registration and login**
* **Broadcast messages** to all online users
* **Private messages** to a specific recipient
* Concurrent clients using **pthread-based threading**

## 🚀 Key Features

* ✅ Terminal-based User Interface
* ✅ Multi-client handling using `pthread`
* ✅ Broadcast and private chat support
* ✅ Basic authentication (username/password)
* ✅ Clean socket handling and message structuring

## 📁 Project Structure

```bash
📦 CN-Chat-Application
├── client.c           # Client-side implementation
├── server.c           # Server-side implementation
├── client             # Compiled client executable
├── server             # Compiled server executable
├── a.out              # Optional leftover compilation file (ignore)
├── *.dSYM             # macOS debug symbol folders (optional, ignore)
└── README.md          # This project description
```

## 💻 Compilation & Execution

```bash
# Step 1: Compile both programs
$ gcc client.c -o client -lpthread
$ gcc server.c -o server -lpthread

# Step 2: Run server in one terminal
$ ./server

# Step 3: Run client in other terminals
$ ./client
```

## 👥 Sample User Flow

* Start server: `Server is running...`
* Client 1: Register as `Teja` → Login → Send Broadcast: "Hi, Welcome to my project Buddy!"
* Client 2: Register as `Ravi` → Login → Private message to `Teja`: "Thank you!"
* Client 3+: Repeat similar flow to interact

## 🛠️ Technologies Used

* **Language:** C
* **Libraries:** POSIX Sockets, `pthread.h`, `arpa/inet.h`, `unistd.h`
* **OS Support:** macOS/Linux (fully terminal-based execution)
* **Editor:** VS Code multi-terminal view (for demo)

## 🔐 License

This project is licensed under the **Apache License 2.0**, which permits:

* ✅ Commercial use
* ✅ Modification
* ✅ Distribution
* ✅ Patent use

📄 See the `LICENSE` file for full legal terms.

## 🎯 Credits

* 👨‍💻 **Sri Vighna Teja** – AIML Student, Sreyas Institute of Engineering and Technology
* 💬 Supported by concepts learned from the CN course and enhanced via online learning resources and self-exploration.
