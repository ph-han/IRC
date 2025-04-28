# IRC
Amaging Internet Relay Chat Server

## Introduction

---

## Features

---

## Prerequisites

---

## Installation

---

## Flow Chart
```mermaid
flowchart TD
    A[Start: main.cpp] --> B[Create Server object]
    B --> C[Server setup: socket, bind, listen]
    C --> D{Server Loop}
    D --> E[Accept Client Connection]
    E --> F[Create UserAccount]
    F --> G[Register UserAccount in Database Singleton]
    D --> H[Receive Client Message]
    H --> I[Parse Message]
    I --> J{Command Dispatcher}
    J --> K1[JOIN Command]
    K1 --> K1a[Check if Channel exists in Database]
    K1a -->|Exists| K1b[Join Channel]
    K1a -->|Not Exists| K1c[Create new Channel and save in Database]
    J --> K2[NICK Command: Update UserAccount nickname]
    J --> K3[PRIVMSG Command: Send message to Channel/User]
    J --> K4[Other Commands: Handle accordingly]
    D --> L[Client Disconnects]
    L --> M[Remove UserAccount from Database]
    M --> D
```

---

## Contributors
<table>
    <tbody>
        <tr>
            <td align="center" valign="top">
                <a href="https://github.com/west-eastH">
                    <img src="https://avatars.githubusercontent.com/u/108206977?v=4" width="150px;" height="150px;" alt="phan"/><br />
                    <sub><b>Seo Donghyeon</b></sub>
                </a>
            </td>
            <td align="center" valign="top">
                <a href="https://github.com/ph-han">
                    <img src="https://avatars.githubusercontent.com/u/58614643?v=4" width="150px;" height="150px;" alt="phan"/><br />
                    <sub><b>Han Pilho</b></sub>
                </a>
            </td>
            <td align="center" valign="top">
                <a href="https://github.com/ph-han">
                    <img src="https://avatars.githubusercontent.com/u/86454797?v=4" width="150px;" height="150px;" alt="phan"/><br />
                    <sub><b>Han Jongmin</b></sub>
                </a>
            </td>
            <td align="center" valign="top">
                <a href="https://github.com/ph-han">
                    <img src="https://avatars.githubusercontent.com/u/66724166?v=4" width="150px;" height="150px;" alt="phan"/><br />
                    <sub><b>Im Hyunsoon</b></sub>
                </a>
            </td>
        </tr>
    </tbody>
</table>
