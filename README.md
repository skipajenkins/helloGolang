
---

### 🐹 Hello Golang

---

This project is a beginner-friendly introduction to Go (Golang).
It demonstrates how to:

* Set up a Go project using modules

* Write and run a basic Go program

* Import and use external packages

* Understand Go’s project structure and entry point

This repository is part of a learning journey similar to Rust’s “Hello, World!” examples — but using idiomatic Go tooling.

---

## 🎯 Learning Objectives

By working through this project, you will learn:

* How Go programs are structured

* How main.go works as the entry point

* How to initialize and use go.mod

* How to import standard and third-party packages

* How to run Go code using the Go toolchain

📁 Project Structure
```bash
hello/
├── go.mod
├── go.sum
├── hello.go
└── README.md
```
File Breakdown
| File | Purpose |
|------|--------|
| go.mod | Defines the Go module |
| go.sum | Tracks dependency versions |
| main.go | Application entry point |


---

## ⚙️ Setting Up the Environment

###✅ Step 1: Install Go

Check if Go is already installed:
```bash
go version
```

If Go is not installed, download it from the official site:

👉 https://go.dev/dl/

Follow the installer instructions for your operating system, then verify again:

```bash
go version
```

---

### 📦 Step 2: Create a Go Project (From Scratch)

If you were creating this project yourself, the steps would be:
```bash
mkdir hello
cd hello
go mod init hello
```

This creates the go.mod file, which enables Go Modules (Go’s dependency system).

---

## 📜 Go Code
```bash
package main

import (
	"fmt"
	"rsc.io/quote"
)

func main() {
	fmt.Println("Hello, World!")
	fmt.Println(quote.Go())
}
```

---

##🧠 Code Explanation

### package main
```bash
package main
```

---

Every executable Go program must use package main.

---

### Imports
```bash
import (
	"fmt"
	"rsc.io/quote"
)
```

* fmt → Standard library package for formatted I/O

* rsc.io/quote → External package providing famous Go quotes

When you run the program, Go automatically downloads this dependency and records it in go.mod and go.sum.

---

### func main()
```bash
func main() {
	fmt.Println("Hello, World!")
	fmt.Println(quote.Go())
}
```

* main() is the entry point of every Go executable

* fmt.Println prints to standard output

* quote.Go() returns a predefined Go-related quote
  
---

## ▶️ Building and Running the Program
### 🧱 Build the Project
```bash
go build
```

This produces a platform-specific executable.

---

### 🎬 Run the Program
```bash
go run hello.go
```

## Example Output
```bash
Hello, World!
Don't communicate by sharing memory, share memory by communicating.
```

## 🧩 Key Concepts Demonstrated
| Concept | Explanation |
|--------|------------|
| Go Modules | Dependency management via `go.mod` |
| Entry Point | `func main()` |
| Imports | Standard + external packages |
| Dependency Fetching | Automatic via `go run` |
| Compilation | Go produces native binaries |

---

## 🚀 Why This Project Exists

This repository serves as:

A Go equivalent to Rust’s early learning projects

A foundation for understanding Go tooling

A reference for future Go projects

A clean example of idiomatic Go setup

---

## 🧾 Built With

* Go (Golang)

* Go Modules

* Standard Library (fmt)

* External Package (rsc.io/quote)

---

## 📄 License

This project is open-source and available under the MIT License.

---
