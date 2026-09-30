<!-- ============================================================= -->
<!--                    NILAM DEV • PROFILE README                 -->
<!-- ============================================================= -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=230&section=header&text=NILAM%20DEV&fontSize=80&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Rust%20•%20DSA%20•%20AWS&descAlignY=60&descSize=26" width="100%" alt="Nilam Dev banner"/>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=F74C00&center=true&vCenter=true&width=600&lines=Learning+Rust+%F0%9F%A6%80;Solving+DSA+Problems+%F0%9F%A7%A9;Exploring+AWS+%E2%98%81%EF%B8%8F;Building+in+public%2C+one+commit+at+a+time" alt="Typing SVG" />
</a>

<br/>

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![DSA](https://img.shields.io/badge/DSA-6C63FF?style=for-the-badge&logo=leetcode&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=FF9900)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=nilamdev01&label=Profile%20Views&color=orange&style=flat-square)
![Followers](https://img.shields.io/github/followers/nilamdev01?label=Followers&style=flat-square&color=blueviolet)
![Stars](https://img.shields.io/github/stars/nilamdev01?label=Stars&style=flat-square&color=yellow)

</div>

---

<div align="center">

### 🧭 Quick Navigation

[**About**](#-about-me) •
[**Focus**](#-current-focus) •
[**Rust**](#-rust) •
[**DSA**](#-data-structures--algorithms) •
[**AWS**](#%EF%B8%8F-aws) •
[**Roadmap**](#%EF%B8%8F-2026-roadmap) •
[**Stats**](#-github-stats) •
[**Connect**](#-lets-connect)

</div>

---

## 👨‍💻 About Me

```rust
struct NilamDev {
    name: &'static str,
    location: &'static str,
    role: &'static str,
    languages: Vec<&'static str>,
    practicing: Vec<&'static str>,
    exploring: Vec<&'static str>,
    motto: &'static str,
}

impl NilamDev {
    fn new() -> Self {
        Self {
            name: "Nilam Dev",
            location: "Bihar, India 🇮🇳",
            role: "Network Engineering Enthusiast",
            languages: vec!["Rust 🦀"],
            practicing: vec![
                "Data Structures",
                "Algorithms",
                "Problem Solving",
            ],
            exploring: vec![
                "AWS ☁️",
                "Cloud Architecture",
                "Networking",
                "Serverless",
            ],
            motto: "Learn. Build. Solve. Repeat.",
        }
    }

    fn say_hi(&self) {
        println!("👋 Hi, I'm {}!", self.name);
        println!("📍 Based in {}", self.location);
        println!("🌐 {}", self.role);
        println!("🎯 {}", self.motto);
    }
}

fn main() {
    let me = NilamDev::new();
    me.say_hi();
}

```

---

## 🎯 Current Focus

<table align="center">
<tr>
<td align="center" width="33%">

### 🦀
### **Rust**
Learning ownership, borrowing, lifetimes and writing safe, fast code.

![progress](https://img.shields.io/badge/Progress-▰▰▰▱▱▱▱▱▱▱_30%25-orange?style=flat-square)

</td>
<td align="center" width="33%">

### 🧩
### **DSA**
Solving problems to sharpen logic, patterns and speed.

![progress](https://img.shields.io/badge/Progress-▰▰▰▰▱▱▱▱▱▱_40%25-blueviolet?style=flat-square)

</td>
<td align="center" width="33%">

### ☁️
### **AWS**
Exploring compute, storage, security and serverless services.

![progress](https://img.shields.io/badge/Progress-▰▰▱▱▱▱▱▱▱▱_20%25-yellow?style=flat-square)

</td>
</tr>
</table>

---

## 🔭 At a Glance

| 🏷️ Category | 📌 Details |
|:---|:---|
| 🦀 **Learning** | Rust programming language |
| 🧩 **Solving** | Data Structures & Algorithms problems |
| ☁️ **Exploring** | AWS cloud services |
| 🌱 **Growing** | Problem solving, system design basics |
| 🎯 **Goal** | Become a confident systems + cloud developer |
| ⚡ **Fun fact** | I fight the borrow checker daily (and sometimes win) |

---

## 🦀 Rust

> *"Fearless concurrency. Zero-cost abstractions. Memory safety without a garbage collector."*

### 📚 What I'm Learning

- [x] Installing Rust & using `cargo`
- [x] Variables, mutability & data types
- [x] Functions & control flow
- [ ] Ownership, borrowing & references
- [ ] Lifetimes
- [ ] Structs, enums & pattern matching
- [ ] `Option` and `Result` error handling
- [ ] Collections: `Vec`, `HashMap`, `HashSet`
- [ ] Traits & generics
- [ ] Iterators & closures
- [ ] Smart pointers: `Box`, `Rc`, `RefCell`
- [ ] Concurrency with threads & channels
- [ ] Async Rust with `tokio`

### 🧪 Sample: Ownership in Action

```rust
fn main() {
    let s1 = String::from("hello");
    let s2 = s1.clone();          // deep copy, both valid
    println!("{s1} {s2}");

    let len = calculate_length(&s1); // borrow, no move
    println!("'{s1}' has length {len}");
}

fn calculate_length(s: &String) -> usize {
    s.len()
}
```

### 🧪 Sample: Pattern Matching

```rust
enum Shape {
    Circle(f64),
    Rectangle(f64, f64),
    Triangle(f64, f64),
}

fn area(shape: &Shape) -> f64 {
    match shape {
        Shape::Circle(r) => std::f64::consts::PI * r * r,
        Shape::Rectangle(w, h) => w * h,
        Shape::Triangle(b, h) => 0.5 * b * h,
    }
}
```

### 🧪 Sample: Error Handling

```rust
use std::fs;
use std::io;

fn read_file(path: &str) -> Result<String, io::Error> {
    let contents = fs::read_to_string(path)?;
    Ok(contents)
}

fn main() {
    match read_file("notes.txt") {
        Ok(text) => println!("{text}"),
        Err(e) => eprintln!("Oops: {e}"),
    }
}
```

<details>
<summary><b>🧠 Rust Concepts Cheat Sheet (click to expand)</b></summary>

<br/>

| Concept | One-line Summary |
|:---|:---|
| **Ownership** | Every value has exactly one owner; dropped when owner goes out of scope |
| **Borrowing** | `&T` shared reference, `&mut T` exclusive reference |
| **Lifetimes** | Compiler-checked scopes that keep references valid |
| **Traits** | Shared behavior, like interfaces |
| **Generics** | Write code once, use it for many types |
| **Enums** | Types that can be one of several variants |
| **`Option<T>`** | Value that may or may not exist (`Some` / `None`) |
| **`Result<T, E>`** | Success (`Ok`) or failure (`Err`) |
| **Cargo** | Build tool + package manager |
| **Crates** | Rust packages published on crates.io |

</details>

### 🛠️ Rust Project Ideas

| # | Project | Difficulty | Status |
|:-:|:---|:-:|:-:|
| 1 | Guessing Game CLI | 🟢 Easy | ✅ Done |
| 2 | To-Do List CLI | 🟢 Easy | 🚧 Planned |
| 3 | Word Counter (`wc` clone) | 🟡 Medium | 🚧 Planned |
| 4 | Mini `grep` in Rust | 🟡 Medium | 🚧 Planned |
| 5 | Simple HTTP Server | 🟠 Hard | 💡 Idea |
| 6 | Key-Value Store | 🟠 Hard | 💡 Idea |
| 7 | AWS S3 CLI Tool in Rust | 🔴 Advanced | 💡 Idea |

---

## 🧩 Data Structures & Algorithms

> *"Talk is cheap. Show me the code."*

### 🗂️ Topics Tracker

| Topic | Status | Problems Solved |
|:---|:-:|:-:|
| 📦 Arrays | ✅ Done | ▰▰▰▰▰▰▰▱▱▱ |
| 🔤 Strings | ✅ Done | ▰▰▰▰▰▰▱▱▱▱ |
| #️⃣ Hashing | 🚧 In Progress | ▰▰▰▰▱▱▱▱▱▱ |
| 👉 Two Pointers | 🚧 In Progress | ▰▰▰▱▱▱▱▱▱▱ |
| 🪟 Sliding Window | 🚧 In Progress | ▰▰▱▱▱▱▱▱▱▱ |
| 🔗 Linked Lists | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 📚 Stacks & Queues | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 🔍 Binary Search | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 🌳 Trees | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 🕸️ Graphs | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 🧮 Dynamic Programming | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| ⛰️ Heaps | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |
| 🔙 Backtracking | ⏳ Upcoming | ▱▱▱▱▱▱▱▱▱▱ |

### ⏱️ Big-O Cheat Sheet

| Data Structure | Access | Search | Insert | Delete |
|:---|:-:|:-:|:-:|:-:|
| Array | O(1) | O(n) | O(n) | O(n) |
| Linked List | O(n) | O(n) | O(1) | O(1) |
| Stack | O(n) | O(n) | O(1) | O(1) |
| Queue | O(n) | O(n) | O(1) | O(1) |
| Hash Table | N/A | O(1) avg | O(1) avg | O(1) avg |
| Binary Search Tree | O(log n) | O(log n) | O(log n) | O(log n) |
| Heap | O(1) top | O(n) | O(log n) | O(log n) |

| Algorithm | Best | Average | Worst |
|:---|:-:|:-:|:-:|
| Binary Search | O(1) | O(log n) | O(log n) |
| Bubble Sort | O(n) | O(n²) | O(n²) |
| Merge Sort | O(n log n) | O(n log n) | O(n log n) |
| Quick Sort | O(n log n) | O(n log n) | O(n²) |
| BFS / DFS | O(V+E) | O(V+E) | O(V+E) |

### 🧪 Sample: Two Sum in Rust

```rust
use std::collections::HashMap;

/// Returns indices of two numbers that add up to `target`.
/// Time: O(n)  |  Space: O(n)
pub fn two_sum(nums: Vec<i32>, target: i32) -> Option<(usize, usize)> {
    let mut seen: HashMap<i32, usize> = HashMap::new();

    for (i, &num) in nums.iter().enumerate() {
        let complement = target - num;
        if let Some(&j) = seen.get(&complement) {
            return Some((j, i));
        }
        seen.insert(num, i);
    }
    None
}

fn main() {
    let result = two_sum(vec![2, 7, 11, 15], 9);
    println!("{:?}", result); // Some((0, 1))
}
```

### 🧪 Sample: Binary Search in Rust

```rust
/// Time: O(log n)  |  Space: O(1)
pub fn binary_search(arr: &[i32], target: i32) -> Option<usize> {
    let (mut low, mut high) = (0usize, arr.len());

    while low < high {
        let mid = low + (high - low) / 2;
        if arr[mid] == target {
            return Some(mid);
        } else if arr[mid] < target {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    None
}
```

### 🧪 Sample: Reverse a Linked List (concept)

```rust
#[derive(Debug)]
struct ListNode {
    val: i32,
    next: Option<Box<ListNode>>,
}

fn reverse_list(head: Option<Box<ListNode>>) -> Option<Box<ListNode>> {
    let mut prev = None;
    let mut curr = head;

    while let Some(mut node) = curr {
        curr = node.next.take();
        node.next = prev;
        prev = Some(node);
    }
    prev
}
```

### 🎯 Problem-Solving Patterns I'm Learning

```mermaid
mindmap
  root((DSA Patterns))
    Arrays
      Two Pointers
      Sliding Window
      Prefix Sum
    Searching
      Binary Search
      BFS
      DFS
    Optimization
      Greedy
      Dynamic Programming
      Backtracking
    Structures
      Stack
      Queue
      Heap
      Trie
```

### 📈 My Problem-Solving Approach

1. 📖 **Understand** the problem, inputs, outputs, edge cases
2. 🧠 **Brute force** first, then think of optimizations
3. 🔍 **Identify the pattern** (two pointers, hashing, DP, etc.)
4. ✍️ **Write** clean code
5. 🧪 **Test** with edge cases
6. ⏱️ **Analyze** time and space complexity
7. 📝 **Review** and note what I learned

---

## ☁️ AWS

> *"There is no cloud, it's just someone else's computer, but a really, really good one."*

### 🧱 Services I'm Exploring

| Category | Service | What It Does | Status |
|:---|:---|:---|:-:|
| 🖥️ Compute | **EC2** | Virtual servers in the cloud | 🚧 |
| ⚡ Compute | **Lambda** | Run code without managing servers | 🚧 |
| 🗄️ Storage | **S3** | Scalable object storage | ✅ |
| 🔐 Security | **IAM** | Users, roles and permissions | 🚧 |
| 🗃️ Database | **DynamoDB** | Serverless NoSQL database | ⏳ |
| 🗃️ Database | **RDS** | Managed relational databases | ⏳ |
| 🌐 Networking | **VPC** | Your private network in AWS | ⏳ |
| 🌍 Networking | **Route 53** | DNS and domain management | ⏳ |
| 🚪 API | **API Gateway** | Create and manage APIs | ⏳ |
| 📊 Monitoring | **CloudWatch** | Logs, metrics and alarms | ⏳ |
| 🏗️ IaC | **CloudFormation** | Infrastructure as code | ⏳ |

### 🏛️ Architecture I'm Working Toward

```mermaid
flowchart LR
    U([👤 User]) --> AG[API Gateway]
    AG --> L[⚡ Lambda<br/>Rust runtime]
    L --> D[(DynamoDB)]
    L --> S[(S3 Bucket)]
    L --> CW[CloudWatch Logs]
    IAM{{IAM Roles}} -.-> L
```

### 🔄 Learning Path

```mermaid
flowchart TD
    A[☁️ Cloud Basics] --> B[🔐 IAM & Security]
    B --> C[🖥️ EC2 & Networking]
    C --> D[🗄️ S3 & Storage]
    D --> E[⚡ Lambda & Serverless]
    E --> F[🗃️ Databases]
    F --> G[🏗️ Infrastructure as Code]
    G --> H[🚀 Deploy a Real Project]
```

### 💡 AWS + Rust = ❤️

Rust is a great fit for the cloud: tiny binaries, fast cold starts, and low memory usage.

```rust
// Idea: a Lambda function written in Rust
use lambda_runtime::{service_fn, Error, LambdaEvent};
use serde_json::{json, Value};

async fn handler(event: LambdaEvent<Value>) -> Result<Value, Error> {
    let name = event.payload["name"].as_str().unwrap_or("world");
    Ok(json!({ "message": format!("Hello, {name}! 🦀☁️") }))
}

#[tokio::main]
async fn main() -> Result<(), Error> {
    lambda_runtime::run(service_fn(handler)).await
}
```

<details>
<summary><b>🔐 AWS Best Practices I'm Keeping in Mind (click to expand)</b></summary>

<br/>

- 🔒 Never use the root account for daily work
- 🔑 Enable **MFA** everywhere
- 🪪 Follow **least privilege** in IAM policies
- 💰 Set up **billing alarms** to avoid surprise costs
- 🧹 Always clean up unused resources
- 🏷️ Tag your resources
- 🚫 Never commit access keys to Git

</details>

---

## 🗺️ 2026 Roadmap

```mermaid
gantt
    title Learning Roadmap
    dateFormat  YYYY-MM-DD
    section 🦀 Rust
    Rust Basics             :done,    r1, 2026-01-01, 45d
    Ownership & Lifetimes   :active,  r2, after r1, 45d
    Traits & Generics       :         r3, after r2, 30d
    Async & Projects        :         r4, after r3, 60d
    section 🧩 DSA
    Arrays & Strings        :done,    d1, 2026-01-01, 40d
    Hashing & Pointers      :active,  d2, after d1, 40d
    Trees & Graphs          :         d3, after d2, 60d
    Dynamic Programming     :         d4, after d3, 60d
    section ☁️ AWS
    Cloud Fundamentals      :active,  a1, 2026-03-01, 45d
    Compute & Storage       :         a2, after a1, 45d
    Serverless              :         a3, after a2, 45d
    Real Project Deploy     :         a4, after a3, 45d
```

---

## 🏆 Goals

| 🎯 Goal | 📅 Target | 📊 Progress |
|:---|:-:|:-:|
| Solve **300+** DSA problems | End of 2026 | ▰▰▱▱▱▱▱▱▱▱ |
| Build **5** Rust projects | End of 2026 | ▰▱▱▱▱▱▱▱▱▱ |
| Deploy **1** project on AWS | Q4 2026 | ▱▱▱▱▱▱▱▱▱▱ |
| Contribute to **open source** | Q4 2026 | ▱▱▱▱▱▱▱▱▱▱ |
| Write **10** learning blog posts | End of 2026 | ▱▱▱▱▱▱▱▱▱▱ |

---

## 📓 Learning Log

<details open>
<summary><b>📅 Recent Progress</b></summary>

<br/>

| Date | What I Did |
|:---|:---|
| 🗓️ Week 1 | Set up Rust toolchain, wrote first `Hello, World!` 🦀 |
| 🗓️ Week 2 | Solved array & string problems, learned `cargo` |
| 🗓️ Week 3 | Started hashing patterns, created AWS free-tier account |
| 🗓️ Week 4 | Explored S3 and IAM basics |
| 🗓️ Week 5 | Studying ownership and borrowing in depth |

*(Update this log regularly! 📝)*

</details>

---

## 📊 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=nilamdev01&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=nilamdev01&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />

<br/>

<img src="https://streak-stats.demolab.com?user=nilamdev01&theme=tokyonight&hide_border=true" alt="GitHub streak" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=nilamdev01&theme=tokyo-night&hide_border=true" alt="Activity graph" width="95%" />

</div>

---

## 🏅 Achievements

<div align="center">

![Trophy](https://github-profile-trophy.vercel.app/?username=nilamdev01&theme=tokyonight&no-frame=true&no-bg=true&margin-w=10)

</div>

---

## 🧰 Tools & Tech

<div align="center">

**Languages**

![Rust](https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Markdown](https://img.shields.io/badge/-Markdown-083fa1?style=flat-square&logo=markdown&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=FF9900)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Tools**

![VS Code](https://img.shields.io/badge/-VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white)
![LeetCode](https://img.shields.io/badge/-LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=black)

</div>

---

## 📚 Resources I Love

| Topic | Resource |
|:---|:---|
| 🦀 Rust | [The Rust Book](https://doc.rust-lang.org/book/) |
| 🦀 Rust | [Rust by Example](https://doc.rust-lang.org/rust-by-example/) |
| 🦀 Rust | [Rustlings](https://github.com/rust-lang/rustlings) |
| 🧩 DSA | [LeetCode](https://leetcode.com) |
| 🧩 DSA | [NeetCode](https://neetcode.io) |
| 🧩 DSA | [GeeksforGeeks](https://www.geeksforgeeks.org) |
| ☁️ AWS | [AWS Documentation](https://docs.aws.amazon.com) |
| ☁️ AWS | [AWS Skill Builder](https://skillbuilder.aws) |

---

## 🤝 Open To

- 🦀 Collaborating on Rust projects
- 🧩 DSA study groups & pair problem-solving
- ☁️ Sharing AWS learning tips
- 🌱 Mentorship and feedback

---

## 💬 Ask Me About

**Rust basics • DSA patterns • Getting started with AWS • Learning consistently**

---

## 📫 Let's Connect

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nilamdev01)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/nilamdev01)
[![Twitter](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/nilamdev01)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your@email.com)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/nilamdev01)

<br/>

### 💭 *"The best time to start was yesterday. The next best time is now."*

<br/>

**⭐ Thanks for visiting my profile! If you like what you see, drop a star. ⭐**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer&text=NILAM%20%E2%9D%A4%EF%B8%8F%20AJIT&fontSize=28&fontColor=ffffff&fontAlignY=65" width="100%" alt="NILAM ❤️ AJIT footer"/>
</div>
