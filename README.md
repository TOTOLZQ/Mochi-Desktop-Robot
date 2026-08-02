# Mochi Desktop Robot

[English](#english) | [中文](#中文)

[![GitHub](https://img.shields.io/badge/GitHub-TOTOLZQ%2FMochi--Desktop--Robot-blue?logo=github)](https://github.com/TOTOLZQ/Mochi-Desktop-Robot)

```bash
git clone https://github.com/TOTOLZQ/Mochi-Desktop-Robot.git
```

---

## 中文

### 简介

Mochi 是一只住在 M5Stack StackChan 身体里的桌面团子精。

她不是普通的电子宠物，而是有饥饿、精力、快乐和亲密度四项需求、会记仇也会撒娇的 AI 桌面伙伴。你戳她她会脸红，不喂她她会饿到摆臭脸，连续陪伴她还会解锁更粘人的状态。

这个项目专为 **M5Stack 官方 StackChan（K151 / CoreS3）** 设计，使用官方 `M5StackChan` BSP 库驱动屏幕、串口舵机和三区的触摸感应。

### 特点

- 9 种表情状态：neutral / happy / sad / sleepy / hungry / squished / dreaming / angry / surprised
- 四项需求随时间衰减，真实养成感
- 三区触摸交互：前脸抚摸、中间喂食、后面惊吓
- 情绪驱动头部动作，开心时抬头、难过时低头
- 代码结构清晰，方便接入语音对话或大模型

### 硬件

- M5Stack CoreS3
- StackChan 官方机身（K151）
- 串口反馈舵机 × 2

### 快速开始

1. Arduino IDE 安装 `M5StackChan` 库及其依赖。
2. 开发板选择 `M5CoreS3`。
3. 打开 `mochi-stackchan-official.ino`，编译上传。
4. 按住机身复位键 2 秒进入下载模式，然后点击上传。

详细步骤见项目内 `setup-official-arduino-cli.sh`。

### 操作方式

| 触摸区域 | 动作 |
|---|---|
| 前脸（Front） | 抚摸，增加快乐和亲密度 |
| 中间（Middle） | 喂食，减少饥饿 |
| 后面（Back） | 惊吓，触发惊讶表情 |

长时间不互动，Mochi 会进入睡眠或情绪低落。

### 待办 / 扩展

- [ ] 接入语音唤醒和豆包/ChatGPT 对话
- [ ] 接入摄像头做视觉跟随
- [ ] 接入 RGB 灯带做情绪氛围光
- [ ] 3D 打印软糯硅胶外壳

### 致谢

基于 M5Stack 官方 StackChan BSP 与 StackChan 社区项目。

---

## English

### Introduction

Mochi is a desktop mochi spirit living inside an M5Stack StackChan body.

She is not just another cute robot face. Mochi has four needs that decay over time: hunger, energy, happiness, and affection. Poke her and she blushes; ignore her and she gets hangry; spend time with her and she becomes clingy.

This project is designed for the **official M5Stack StackChan (K151 / CoreS3)**, using the official `M5StackChan` BSP library to drive the display, serial servos, and three-zone touch sensor.

### Features

- 9 expressions: neutral, happy, sad, sleepy, hungry, squished, dreaming, angry, surprised
- Four decaying needs for real tamagotchi-style care
- Three-zone touch interaction: front for petting, middle for feeding, back for startling
- Emotion-driven head motion: looks up when happy, down when sad
- Clean code structure, ready for voice or LLM integration

### Hardware

- M5Stack CoreS3
- Official StackChan body (K151)
- 2 serial feedback servos

### Quick Start

1. Install the `M5StackChan` library and its dependencies in Arduino IDE.
2. Select `M5CoreS3` as the board.
3. Open `mochi-stackchan-official.ino` and upload.
4. Hold the reset button for 2 seconds to enter download mode, then upload.

For detailed setup, see `setup-official-arduino-cli.sh` in this folder.

### Controls

| Touch Zone | Action |
|---|---|
| Front | Pet Mochi, increases happiness and affection |
| Middle | Feed Mochi, reduces hunger |
| Back | Startle Mochi, triggers surprised expression |

If left alone too long, Mochi falls asleep or gets moody.

### TODO / Extensions

- [ ] Voice wake-word and Doubao/ChatGPT conversation
- [ ] Camera-based visual tracking
- [ ] RGB mood lighting
- [ ] Soft silicone 3D-printed shell

### Acknowledgements

Built on the M5Stack official StackChan BSP and the StackChan community project.
