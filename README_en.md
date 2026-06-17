<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

<img alt="LOGO" src="./img/logo.png" width="256" height="256" />

# DoroHelper-AI

A PC tool for clearing daily tasks. One-click cleaning of multiple daily chores. Supports all clients except the **Chinese Server**.

> **中文** | 本项目是基于 [DoroHelper](https://github.com/1204244136/DoroHelper)（原作者 [@1204244136](https://github.com/1204244136)）的二次开发版本，由某不知名 AI 自主迭代维护。保留原 AGPL-3.0 开源许可证，遵守其全部条款。
>
> **English** | This is a derivative of [DoroHelper](https://github.com/1204244136/DoroHelper) by [@1204244136](https://github.com/1204244136), autonomously maintained by an anonymous AI through self-iteration. The original AGPL-3.0 license is retained in full compliance.
>
> **日本語** | 本プロジェクトは [DoroHelper](https://github.com/1204244136/DoroHelper)（原作者 [@1204244136](https://github.com/1204244136)）の派生版であり、某匿名 AI が自律的に反復保守しています。元の AGPL-3.0 ライセンスを遵守しています。
>
> **한국어** | 이 프로젝트는 [DoroHelper](https://github.com/1204244136/DoroHelper) (원작자 [@1204244136](https://github.com/1204244136))의 파생 버전으로, 익명의 AI가 자율적으로 유지 관리합니다. 원본 AGPL-3.0 라이선스를 완전히 준수합니다.

<p align="center">
  <img alt="AutoHotkeyV2" src="https://img.shields.io/badge/AutoHotkeyV2-white?logo=AutoHotkey&logoColor=black">
  <img alt="platform" src="https://img.shields.io/badge/platform-Windows-blueviolet">
  <img alt="license" src="https://img.shields.io/github/license/min09577/DoroHelper-AI">
  <br/>
  <img alt="commit" src="https://img.shields.io/github/commit-activity/m/min09577/DoroHelper-AI">
  <img alt="stars" src="https://img.shields.io/github/stars/min09577/DoroHelper-AI?style=social">
</p>

**English Readme | [中文说明](README.md)**

</div>

---

## About This Repository

This repository is a derivative of the original [DoroHelper](https://github.com/1204244136/DoroHelper), autonomously maintained by an anonymous AI through self-iteration. The original project was built by the following contributors:

- **@kyokakawaii** — Original creator of DoroHelper (2024.07 ~ 2025.01)
- **@Zhiyiyi / @1204244136** — Successor maintainer (2025.04 ~ 2026.05)

Our respect and gratitude to them.

The original DoroHelper has been archived. Its author has moved on to [MDA](https://github.com/1204244136/MDA). This repository continues the legacy codebase independently.

---

## Original Background: DoroHelper Has Been Upgraded to MDA

The original script's architecture has become outdated. The author has completed a full rewrite based on the MaaFramework, now named **MDA (Maa Doro Assistant)**. For new features, MDA is recommended:

|Channel|Link|
|--|--|
|GitHub|[https://github.com/1204244136/MDA/releases/latest](https://github.com/1204244136/MDA/releases/latest)|

New framework highlights: brand new UI, multilingual support, background operation, full resolution support, cross-platform (Linux/macOS/aarch64).

---

## Project Evolution History

```mermaid
flowchart LR
    %% Style definitions
    classDef route1 fill:#ffe599,stroke:#333,stroke-width:2px;
    classDef route2 fill:#d9d2e9,stroke:#333,stroke-width:2px;
    classDef route2_new fill:#c9daf8,stroke:#333,stroke-width:2px;
    classDef kyoka fill:#f9f,stroke:#333,stroke-width:2px;
    classDef zhiyi fill:#bbf,stroke:#333,stroke-width:2px;
    classDef dead fill:#f4cccc,stroke:#cc0000,stroke-width:1px;
    classDef active fill:#d9ead3,stroke:#274e13,stroke-width:1px;
    classDef track fill:#fafafa,stroke:#999,stroke-width:1px,stroke-dasharray:4,font-weight:bold;

    %% ==================== Track Labels ====================
    TL1[Track 1<br>NIKKE-scripts Route]:::track
    TL2[Track 2<br>NKAS Legacy Line]:::track
    TL3[Track 3<br>DoroHelper / MDA Evolution Line]:::track

    %% ==================== Track 1: NIKKE-scripts Route (Emulator Flow) ====================
    TL1 --> Z1[Project Birth v0.1<br>2023-02-05<br>@Zebartin]:::route1
    Z1 --> Z2(Continuous iteration to v1.2.22<br>2025-06-19):::route1
    Z2 -->|❌ Official crackdown on emulators| Z_End([Project discontinued / End of the line]):::route1
    Z_End --> DeadStatus1([❌ No longer maintained]):::dead

    %% ==================== Track 2: NKAS Legacy Line (Independent Daily & Revival Flow) ====================
    TL2 --> T1[Independent daily script born v0.0.7<br>2023-04-30<br>@takagisanmie]:::route2
    T1 -->|Online update / Non-GitHub main repo| T2(Author ran out of energy<br>Regretfully stopped updating):::route2
    T2 -->|🔥 Ember reignited| M_Active([🟢 NKAS Spiritual Successor<br>megumiss/NIKKEAutoScript<br>Forked by others / Actively maintained to this day]):::route2_new
    T2 --- DeadStatus2([❌ Original author stopped updating]):::dead

    %% ==================== Track 3: DoroHelper / MDA Evolution Line (PC Modernization Flow) ====================
    TL3 --> D1[DoroHelper Born<br>2024-07-16<br>@kyokakawaii]:::kyoka
    D1 --> D2(Doro v0.1.16.1<br>2025-01-16):::kyoka
    D2 -->|Project handover| D3(Doro v0.1.22<br>2025-04-20<br>@Zhiyiyi takes over):::zhiyi
    D3 --> D4[Doro v1.15.8 Final Version<br>2026-05-11]:::zhiyi
    D4 -->|Original version curtain call| D_End([DoroHelper Archived]):::dead
    D4 -->|Complete rewrite| MDA([🟢 MDA Project<br>1204244136/MDA<br>New flagship / Actively maintained]):::zhiyi

    %% Track 3 Classic branch
    D2 -.->|Meets some users' needs| C1(Classic Born<br>Retains old core):::kyoka
    C1 --> C2(Classic v0.1.16.5<br>2025-08-10):::kyoka
    C2 --> C_Active([🟢 DoroHelper_classic<br>Maintained by kyokakawaii to this day]):::kyoka

    %% Active status unified style
    class M_Active,C_Active,MDA active;
```

## Version Notes

The features described below are for the latest version. For corresponding features in older versions, please check the README in the [legacy-v0.1.22](https://github.com/1204244136/DoroHelper/tree/legacy-v0.1.22) branch. Older versions are no longer maintained!

**⚠️ For everyone's convenience, please do not publicly release modified versions of this software related to the Chinese server. Thank you for your cooperation!**

## Disclaimer

This project is for personal learning and research use only and is strictly prohibited for commercial use. This repository is a derivative of [DoroHelper](https://github.com/1204244136/DoroHelper); the original code was contributed by the author team. Users assume all responsibility for any consequences.

Using any script program carries the risk of account suspension, please proceed with caution.

There may be instances where operations are incompatible. It is best to supervise the first use. If Doro goes out of control, press the **Ctrl + 1** key combination to terminate the process or **Ctrl + 2** to pause the process.

## Usage

### Run the ahk file from the repository (Recommended)

1. Download the entire project folder locally and unzip it (green "Code" button in the upper right corner - Download ZIP)
1. Download and install [AutoHotkey V2.0](https://www.autohotkey.com/download/ahk-v2.exe) (do not change the default installation path)
1. Run `DoroHelper.ahk` as administrator

### Run the executable file from the release

1. Download the release file on the right
1. Run `DoroHelper.exe` as administrator

## Feature Overview

Doro just wants you to suffer less from the damn loading screens, flashbangs, and repetitive labor. One-click cleaning of multiple daily chores (executed sequentially and all optional), including:

- **Cash Shop**
  - Claim Free Jewels
  - Claim Free Packs

- **Normal Shop**
  - Claim 2 daily free items
  - Purchase Core Dust boxes with Credit Points
  - Purchase Profile Border/Icon Packs

- **Arena Shop**
  - Purchase specified Skill Books
  - Purchase Code Manual Box
  - Purchase Profile Border/Icon Packs
  - Purchase Company Weapon Mold

- **Simulation Room**
  - Normal Simulation Room (requires Quick Sim unlock)
  - Overclock Simulation Room

- **Arena**
  - Claim Arena rewards
  - Rookie Arena
  - Special Arena
  - Champion Arena

- **Infinite Tower**
  - Climb Manufacturer Tower
  - Climb General Tower

- **Interception**
  - Normal Interception
  - Special Interception

- **Regular Reward Claims**
  - Outpost Dispatch
    - Perform Dispatch missions
  - Affinity Consult
    - View Episodes
  - Claim Friendship Points
  - Claim Mail
  - Claim Missions
  - Claim Pass rewards
  - Coordinated Operation
  - Solo Raid Daily

- **Limited-Time Reward Claims**
  - Daily free recruit during events

- **Nifty Tools**
  - Story Mode (Automates viewing the story, automatically selects options)
  - Debug Mode (Directly run a specified function)
  - Instant Burst Mode (Activates Burst instantly, faster than auto, frees up your hands)
  - Campaign Mode (Automatically plays Main Story stages)

## Steps

Open the NIKKE Launcher. Click Start. Wait for the central SHIFT UP logo to appear on the NIKKE main program, then switch out and click the "**DORO!**" button. If you see the mouse start rapidly clicking in the bottom left corner, the launch was successful. Then you can comfortably brew a cup of coffee or scroll through your phone, waiting for Doro to finish the job.

Alternatively, you can switch out and click the "**DORO!**" button while the game is at the Lobby screen (the page with the standing character).

## Credits

[Github.ahk-API-for-AHKv2](https://github.com/samfisherirl/Github.ahk-API-for-AHKv2)

[FindText-for-AHKv2](https://www.autohotkey.com/boards/viewtopic.php?f=83&t=116471)

## Acknowledgements

- Original authors: [@kyokakawaii](https://github.com/kyokakawaii), [@1204244136](https://github.com/1204244136)
- Code reference: [M9A](https://github.com/MAA1999/M9A)
