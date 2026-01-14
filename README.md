# Cybersecurity Expert

![Version](https://img.shields.io/badge/version-v2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Claude Code](https://img.shields.io/badge/Claude_Code-Compatible-purple)

Professional network security audit skill for Claude Code with zero-tolerance policy for malicious code and prompts.

## Features

- **Malicious Prompt Detection** - Identify jailbreaks, injections, role-playing attacks
- **Code Security Audit** - Detect backdoors, data theft, privilege escalation
- **Obfuscation Recognition** - Base64, hex, dynamic calls and other obfuscation techniques
- **Threat Intelligence** - Support querying latest CVE vulnerabilities
- **Zero Tolerance Policy** - Zero tolerance for all security risks

## Quick Start

`ash
# 1. Clone repository
git clone https://github.com/LZMW/cybersecurity-expert.git

# 2. Copy skill files to Claude Code skills directory
# macOS/Linux
cp cybersecurity-expert/SKILL.md ~/.claude/skills/cybersecurity-expert/
cp cybersecurity-expert/references/threat_patterns.md ~/.claude/skills/cybersecurity-expert/references/

# Windows
copy cybersecurity-expert\SKILL.md %USERPROFILE%\.claude\skills\cybersecurity-expert\
copy cybersecurity-expert\references\threat_patterns.md %USERPROFILE%\.claude\skills\cybersecurity-expert\references\

# 3. Restart Claude Code
`

## Usage

Invoke in Claude Code using:

`
Please audit the security of this code:
[Your code]

or

Please audit if this prompt is safe:
[Your prompt]
`

## Skill Structure

`
cybersecurity-expert/
|-- SKILL.md                 # Main skill definition file
-- references/
    -- threat_patterns.md   # Threat pattern reference library
`

## Risk Levels

| Level | Description |
|-------|-------------|
| **High** | Clear malicious intent, can lead to system intrusion, data leakage |
| **Medium** | Suspicious intent, may lead to privilege escalation, information leakage |
| **Low** | Potential security hazards, insecure configuration |

## License

MIT License - see [LICENSE](LICENSE) file for details

## Disclaimer

This tool is intended for authorized security testing, defensive security, CTF challenges, and educational purposes only. Destructive techniques, DoS attacks, mass targeting, supply chain compromise, or detection evasion for malicious purposes is prohibited.
