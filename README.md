# Karpathy-Inspired Claude Code Guidelines

A practical reference for keeping AI-assisted coding focused, simple, and verifiable. The principles are inspired by Andrej Karpathy's observations about common LLM coding mistakes and the [forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills) project referenced in this repository's history.

## Repository status

This repository currently contains this README only. Its previous README was removed in [commit 9f43c8d](https://github.com/ayazaltai/Andrej-Karpathy-Inspired-Claude-Code-Guidelines-/commit/9f43c8d7a4ec6af4d161c49ededfbff5dbd07d22). There is no local application, installable plugin, `CLAUDE.md`, or Cursor rule bundled here.

## Four principles

| Principle | Practical application |
| --- | --- |
| Think before coding | Make assumptions visible, identify ambiguity, and resolve decisions that affect the implementation. |
| Prefer simplicity | Implement the requested behavior with the smallest clear solution; introduce abstractions when an actual use requires them. |
| Keep changes focused | Follow the surrounding style and limit edits to the task. Remove unused code introduced by your own changes. |
| Define verifiable outcomes | Turn the request into observable success criteria, then use appropriate checks to establish whether they are met. |

## Apply the guidance

1. Describe the desired behavior and the files or systems involved.
2. Define how completion will be checked: a reproduced bug, an expected output, a passing check, or a reviewed diff.
3. Add relevant project conventions to your coding assistant's project instructions. For Claude Code, maintain these in your project's `CLAUDE.md`.
4. Ask the assistant to implement a focused change, run the relevant checks, and explain any remaining limitations.

For example:

```text
Fix the empty-list crash in the existing function.
Preserve the public API and surrounding style.
Verify empty input and a normal non-empty input.
Report the changed behavior and the checks you ran.
```

Use judgment for small edits; the amount of planning and verification should match the change.

## Sources and scope

- [Original guidelines project](https://github.com/forrestchang/andrej-karpathy-skills): refer there for its maintained instruction files and installation options.
- [Earlier README in this repository](https://github.com/ayazaltai/Andrej-Karpathy-Inspired-Claude-Code-Guidelines-/blob/6f06e165ffe69697e1d75f7b7e2965f5978c6140/README.md): historical context.

This is an independent reference, with no claim of endorsement by Andrej Karpathy or Anthropic. No standalone license file is currently included in this repository; consult the original project's license before reusing its files.
