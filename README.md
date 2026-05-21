<div align="center">

# 🦴 homo-caveman

> *Same brain, fewer tokens. Now for DeepSeek.*

[![License](https://img.shields.io/badge/License-Commercial-red)](LICENSE)
[![DeepSeek](https://img.shields.io/badge/DeepSeek-Compatible-blue)]()
[![Version](https://img.shields.io/badge/version-1.0.0-green)]()

**Token compression for DeepSeek.** Cuts 60-75% output tokens. 6 compression levels including Classical Chinese. Works with DeepSeek V4, ChatGPT, Claude.

[Examples](#-examples) · [Pricing](#-pricing) · [Quick Start](#-quick-start) · [Why](#-why-homo-caveman) · [Levels](#-compression-levels)

</div>

---

## Examples

**Input:** "Why does my React component re-render?"

**Normal (500 tokens):**
> Your component re-renders because you create a new object reference each render. Wrapping it in useMemo will fix it.

**Homo-Caveman Ultra (120 tokens, -76%):**
> Inline obj prop → new ref → re-render. `useMemo`.

**Input:** "解释数据库连接池"

**Normal (400 tokens):**
> 数据库连接池是一种维护多个数据库连接的技术...

**Homo-Caveman Wenyan (80 tokens, -80%):**
> 池存连接不复建。复用免握手，高负载下仍迅捷。

---

## 💰 Pricing

| Version | Features | Price |
|---------|----------|:-----:|
| **Personal** 🆓 | Full compression, watermarked output, 30-day key | **Free** (email required) |
| **Pro** 🚀 | No watermark, custom rules, priority support | **¥99/year** |
| **Enterprise** 🏢 | SSO, custom adapters, SLA, private deployment | **¥999/year** |

> **Get free personal key:** Email 16208204@qq.com with subject "homo-caveman free"

---

## 🛡️ Source Protection

This repository contains compiled prototypes only. Core compression engine is protected:
- Production builds require a valid license key (`HOMO_LICENSE_KEY`)
- Enterprise deployment uses a private registry, not public source
- Reverse engineering or removal of license checks is prohibited by law

---

## Quick Start

```bash
git clone https://github.com/sevenliuhu/homo-caveman.git
cd homo-caveman

# Use with DeepSeek
python3 compress.py "Your long text" --level ultra
```

---

## Why Homo-Caveman

| Feature | Caveman (Claude only) | Homo-Caveman |
|---------|:---------------------:|:-------------:|
| DeepSeek V4 | ❌ | ✅ |
| ChatGPT | ❌ | ✅ |
| Claude | ✅ | ✅ |
| Chinese Wenyan | ✅ | ✅ Enhanced |
| Chinese Baihua | ❌ | ✅ |
| Watermark-free | ✅ (OSS) | ✅ Pro+ |
| Custom levels | ❌ | ✅ Pro+ |

---

## Business Contact

**HOMO AI**

| Contact | Info |
|---------|------|
| Email | 16208204@qq.com |
| Free key | Email us with project name |
| Enterprise | Custom pricing, private deployment |

> Built on shoulders of [caveman](https://github.com/JuliusBrussee/caveman) (62k⭐). Homage, not clone.
