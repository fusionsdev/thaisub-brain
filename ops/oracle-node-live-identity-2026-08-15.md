---
type: ops
updated: 2026-08-15
---

# ORACLE-NODE live identity

เครื่องนี้คือ **ORACLE-NODE** = `192.168.1.149` (WSL2 Ubuntu, user `barbara`, mirrored).

**Mac Mini M4** เป็นเครื่องแยก ยังมีชีวิต ที่ **`192.168.1.100`** (`fusions-Mac-mini.local` / `MAC-785D33`; SSH `:22`, SMB `:445`, VNC `:5900`) — ไม่ใช่เครื่องนี้ และไม่ใช่ FUSION-CORE.

**FUSION-CORE `192.168.1.101` ตาย** — มีแค่ใน hosts. อย่าใส่ `.101` บน NIC นี้. เข้า WSL ใช้ `wsl` หรือ SSH พอร์ต `22` บน `.149`.

ยังไม่มี distro `Ubuntu-Fusion`. Fusion `ext4.vhdx` ยังอยู่ใน NAS Active Backup (`2.img`).

`V:\\RADIO` หาย. MCP wrappers: `C:\\Users\\Barbara\\.local\\bin\\hermes-mcp.cmd` และ `oracle-mcp-v2.cmd`. Oracle Brain ยังอยู่ `http://192.168.1.69:47778`.
