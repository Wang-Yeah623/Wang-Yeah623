> 🦈 **Pull Shark** — unlocked via 3 merged PRs across [openclaw](https://github.com/openclaw/openclaw) (376k ⭐) and [larksuite/cli](https://github.com/larksuite/cli) (12.6k ⭐).
# Hi, I'm WJzz1 👋

Patience-driven engineer who reads code carefully and writes tests before the fix.

---

## 🚀 Open Source Contributions

### [openclaw/openclaw](https://github.com/openclaw/openclaw) — Personal AI assistant · ⭐ 376k

- **[#89297](https://github.com/openclaw/openclaw/pull/89297)** ✅ *merged* — `docs: add ClawHub CLI page`
  Added a documentation page for the ClawHub CLI to the project's docs.

### [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — "The agent that grows with you" · ⭐ 177k

- **[#37161](https://github.com/NousResearch/hermes-agent/pull/37161)** 🔍 *open · in review* — `docs(readme): sync zh-CN install notes`
  Synced the Simplified-Chinese install instructions in the README with the English version.

### [larksuite/cli](https://github.com/larksuite/cli) — Official Feishu/Lark CLI · ⭐ 12.6k

- **[#1054](https://github.com/larksuite/cli/pull/1054)** ✅ *merged* — `fix(contact): add actionable hint when fanout search all-fail with no API code`
  Filled the only empty `Hint` in `shortcuts/`, so AI agents parsing the JSON error envelope get an actionable next step instead of an empty string. Includes a regression test.

- **[#1037](https://github.com/larksuite/cli/pull/1037)** ✅ *merged* — `fix(common): escape special chars in multipart form filenames`
  Removed a custom `MultipartWriter.CreateFormFile` that bypassed the stdlib's quote escaping, fixing malformed `Content-Disposition` headers for filenames containing `"` or `\`. Covered with table-driven tests.

- **[#1136](https://github.com/larksuite/cli/pull/1136)** 🔍 *open · in review* — `docs(common): sync ParseResourceURL doc comment with new URL prefixes`
  Kept the public doc comment in sync with the actual supported URL prefixes.

---

> *"every error message you write will be parsed by an AI to decide its next action."* — [AGENTS.md, larksuite/cli](https://github.com/larksuite/cli/blob/main/AGENTS.md)
