# deslop-en

An agent skill (Claude Code and other tools that read `SKILL.md`) that removes AI writing patterns from English prose while keeping every claim the text makes.

It is a modified version of [blader/humanizer](https://github.com/blader/humanizer) 4.0.0 by Siqi Chen, released under the MIT license.

## What changed from humanizer

- New section on defensive writing: corrective framings ("does not establish that", "should not be confused with"), boilerplate caveats, process assurances ("carefully reviewed"), and narrated candor.
- New rules for semicolon overuse, colon reveals ("The result: ..."), and the uniform 8 to 20 word sentence band that newer models use in place of em dashes.
- New academic-register section: common boilerplate in papers and abstracts, plus the hedges, semicolons, and passive voice that academic writing legitimately keeps.
- A "never add" list so rewrites do not invent details, opinions, or a fake casual voice.
- A detect-only mode.
- All before/after examples rewritten from scratch. The upstream examples were partly drawn from Wikipedia articles.
- Patterns renumbered and regrouped (§1 to §35).

## Install

Claude Code, user-level:

```bash
git clone https://github.com/icode499/deslop-en.git ~/.claude/skills/deslop-en
```

Or per project: clone into `.claude/skills/deslop-en/` in the repository.

## Use

```
/deslop-en
<paste text>
```

Natural language also works: "deslop this paragraph", "audit draft.md for AI tells, don't rewrite", "clean up the AI patterns in README.md".

## Sources

- [blader/humanizer](https://github.com/blader/humanizer) (MIT): structure, process, and many of the patterns.
- Wikipedia, [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), WikiProject AI Cleanup: pattern research, including the mid-2026 corrective framings and the sentence-length band. Only short phrases are quoted.
- [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) (MIT): ideas for narrated candor, colon reveals, and the "never add" list. No text was copied.

## License

MIT. See [LICENSE](LICENSE).
