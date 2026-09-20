# gpt-skills

A small staged collection of reusable skills for evidence, learning, agent instructions, and prose. The collection favors preservation rules and concrete failure checks over generic task prompts.

| Skill | Use it for |
|---|---|
| `evidence-integrity` | Audit claim support or synthesize sources with traceable attribution |
| `source-tutor` | Teach and assess against a designated source |
| `instruction-audit` | Diagnose and repair instruction rules that produce unintended behavior |
| `natural-writing` | Draft or revise prose while preserving meaning, voice and edit scope |

See [the design document](docs/design.md) for selection decisions, detailed boundaries, multilingual architecture and rejected candidates. See [validation](docs/validation.md) for what was actually checked and what remains unproven.

Each folder under `skills/` is self-contained. `SKILL.md` is the entrypoint; load its references only for the indicated task. `agents/openai.yaml` provides optional Codex UI metadata. No skill requires another skill, a specific model version, a network service, a script, or the maintainer documents. English and Turkish are the only bundled language modules; other languages have no dedicated reviewed module in this version.

For use in a compatible skill host, add only the individual skill folders you want, following that host's installation procedure. Do not load this whole repository as a universal instruction file.

Maintainer evaluations live in [evals/](evals/README.md), outside runtime instruction paths. Expand instructions only for demonstrated recurring failures. Broader model comparisons and competent language review remain release work, not completed validation.

## License

MIT. See [LICENSE](LICENSE).
