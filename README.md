# Hi, I'm WJzz1 👋

Patience-driven engineer who reads code carefully and writes tests before the fix.

---

## 🚀 Open Source Contributions

### [larksuite/cli](https://github.com/larksuite/cli) — Official Feishu/Lark CLI · ⭐ 12.6k

The official CLI tool for Feishu/Lark, maintained by the larksuite team and shipped to AI Agents (Claude Code, Cursor, Gemini CLI).

- **[#1054](https://github.com/larksuite/cli/pull/1054)** ✅ *merged* — `fix(contact): add actionable hint when fanout search all-fail with no API code`
  Found the only `output.ErrWithHint` call in `shortcuts/` shipping an empty `Hint`. AI agents that parse the JSON error envelope now get an actionable next step (*"retry; if it persists, narrow `--queries` to a single term"*) instead of an empty string. Includes a regression test that fails on `main` and passes on the fix.

- **[#1037](https://github.com/larksuite/cli/pull/1037)** 🔍 *in review* — `fix(common): escape special chars in multipart form filenames`
  Removed a custom `MultipartWriter.CreateFormFile` override that bypassed the stdlib's quote escaping — so filenames containing `"`, `\`, CR, or LF produced a malformed `Content-Disposition` header (servers parsed `report "draft".pdf` as `filename="report "`, dropping the rest). Covered with 8 table-driven cases asserting both the on-wire encoding and round-trip through `mime.ParseMediaType`.

---

## 🛠 Tech I work with

- **Languages**: Go · Rust · TypeScript
- **Practices**: Test-driven development · Conventional Commits · Code review with CodeRabbit
- **Areas of interest**: CLI ergonomics · AI Agent tooling · Developer experience

---

## 📊 GitHub

![Wang-Yeah623's GitHub stats](https://github-readme-stats.vercel.app/api?username=Wang-Yeah623&show_icons=true&theme=tokyonight&hide_border=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Wang-Yeah623&layout=compact&theme=tokyonight&hide_border=true)

---

> *"every error message you write will be parsed by an AI to decide its next action."* — [AGENTS.md, larksuite/cli](https://github.com/larksuite/cli/blob/main/AGENTS.md)
