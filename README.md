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
    F --> G[Register User in Database]
    D --> H[Receive Client Message]
    H --> I[Parse Message]
    I --> J{Command Dispatcher}
    J --> K1[JOIN Command: Channel join/create via Channel Manager]
    J --> K2[NICK Command: Update UserAccount nickname]
    J --> K3[PRIVMSG Command: Send message to Channel/User]
    J --> K4[Other Commands: Handle accordingly]
    D --> L[Disconnect Client: Clean up Database/UserAccount]
    L --> D
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
