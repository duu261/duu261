# Duu

**AI agents** · **Neovim** · `Arch` · `tmux` · TUI and CLI over GUI bloat

> Small tools for my own setup. I keep the ones that survive a few weeks of daily use.

### How I build

1. **Check first.** Before a single line: does it exist, or is upstream about to ship it? "Wait" or "use what's there" is a fine answer.
2. **Earn the build.** Will I still want to maintain it in six months? Does anyone besides me need it? Do I actually need it?
3. **Smallest thing that works.** Stdlib over dependency, config over code, a thin overlay on upstream over a fork I'll be rebasing forever.
4. **Mirror upstream.** If the host already does part of the job, follow how it does it. Don't invent a parallel version.
5. **Fail loud and boring.** Risky stuff gets tested against the real service. Low-stakes stuff gets no ceremony.

I break these more than I'd like. Agents finish a working tool in one session, so it's tempting to just build. But code got cheap to write, not cheap to own. The session ends, upstream ships a release, and the drift is mine.

### On agents

I use them daily and trust them about as far as I can check them.

- One agent in charge, bounded workers, me reading the diff.
- Fully autonomous pipelines demo well and are miserable to debug.
- An agent saying *"done"* is not evidence. Tool output is.

Most of my agent tooling exists to close that last gap.
