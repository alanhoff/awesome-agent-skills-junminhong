# Contributing to Awesome Agent Skills

Thank you for helping keep this directory useful and accurate.

> [!IMPORTANT]
> Awesome Agent Skills is a links-only curated directory. A normal listing pull request edits only the two top-level files `README.md` and `README_ZH.md`. Keep skill implementations, `SKILL.md`, scripts, assets, and platform indexes in the upstream project.

## Ways to Contribute

- Add one new project to the directory.
- Correct, update, move, or remove an existing listing.
- Improve the repository documentation or contribution process.
- Report a broken link or propose a new category through an issue.

Listing changes follow the two-file rule above. A focused documentation or repository-maintenance pull request may change other relevant files.

## Eligibility

A listed project must:

- Have a public, canonical source that reviewers can inspect and use.
- Provide a working implementation, not only a product page, announcement, prompt example, or roadmap.
- Explain its purpose, installation or setup, usage, dependencies, required permissions, and external services well enough to evaluate it.
- Include a clear license for the linked implementation.
- Make a concrete Agent workflow possible; a general AI product with no Agent-specific integration is out of scope.
- Support every platform claimed in the listing according to its upstream documentation.
- Have a stable, factual description that does not depend on prices, version numbers, item counts, star counts, or superlatives.

Additional requirements by type:

- **Skill** — includes a directly usable `SKILL.md` and any resources needed for its documented workflow.
- **Collection** — includes multiple directly usable Agent Skills, rather than a list of links to other projects.
- **Tooling or integration** — provides a working plugin, CLI, MCP integration, or similar implementation designed for Agent workflows.

Self-nominations and commercial projects are allowed. Disclose your affiliation or commercial relationship in the pull request and keep the directory description neutral. There is no minimum star count, but meeting the checklist does not guarantee inclusion; maintainers may decline entries that do not fit the directory or add enough distinct value.

## Types and Placement

Use the narrowest accurate type and place the entry in the matching section.

| Project kind | `Type` metadata | README section |
| --- | --- | --- |
| One directly usable skill | `Skill` | Agent Skills, under its functional category |
| Multiple skills maintained together | `Collection` | Skill Collections |
| Agent plugin, CLI, MCP integration, or supporting tool | The concrete type, such as `Plugin`, `CLI`, or `MCP` | Tooling & Integrations |
| A project spanning two types | Join both with ` + `, such as `Plugin + Skill` | The section representing its primary use |

If no existing top-level category or type fits, open an issue and agree on the taxonomy before submitting the listing.

## Listing Format

Use exactly one bullet per project:

```markdown
- [Project name](canonical public source) — One concise, factual description. `Type: Skill` · `Platforms: Cross-platform`
```

Follow these rules:

- Link to the canonical repository. For a monorepo, link directly to the relevant skill or collection directory.
- Write one sentence describing what the project lets an Agent do.
- Use `Cross-platform` only when upstream documentation supports multiple Agent hosts; otherwise list the documented hosts by name.
- Sort entries alphabetically by visible project name within each subsection, ignoring letter case.
- Keep the visible name, URL, `Type`, and `Platforms` text identical in both READMEs. Translate only the prose description and surrounding documentation.
- Update an existing entry instead of adding a duplicate when a project is renamed, transferred, or moved.

## Pull Request Scope

For a listing addition, update, move, or removal:

- Change only `README.md` and `README_ZH.md`.
- Keep both language versions synchronized in the same pull request.
- Submit one upstream project, or one tightly related collection maintained as a unit, per pull request.
- Do not add a local `skills/` tree, `SKILL.md`, scripts, generated files, copied assets, or platform-specific README files.
- Do not combine unrelated documentation or repository changes with the listing.

For documentation or repository-maintenance work, change only the files needed for that work and explain the scope in the pull request.

## Submission Workflow

1. Search the READMEs, open issues, and open pull requests for duplicates or earlier discussion.
2. Verify the canonical URL, implementation, documentation, license, and stated platform support.
3. Add or update the entry in the correct section of both READMEs.
4. Confirm the two entries have matching names, URLs, types, and platforms and are alphabetized.
5. Open a focused pull request, preferably titled `docs: add <project-name>` for a new listing.
6. State your affiliation with the project or write `None`.
7. Ensure **every commit** in the pull request displays **Verified** on GitHub. See [GitHub's guide to signing commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits).

## Listing Checklist

Before requesting review, confirm that:

- [ ] The canonical source, implementation, documentation, and license are public and working.
- [ ] The project meets the requirements for its stated type.
- [ ] Platform claims are supported by upstream documentation.
- [ ] The description is concise, factual, neutral, and unlikely to become stale quickly.
- [ ] The entry is not a duplicate and is alphabetized in the correct section.
- [ ] `README.md` and `README_ZH.md` contain matching metadata.
- [ ] The pull request covers one project and changes only those two files.
- [ ] No upstream skill files or supporting assets are copied into this repository.
- [ ] Any affiliation or commercial relationship is disclosed.
- [ ] Every commit displays Verified on GitHub.

## Updating or Removing a Listing

Submit a two-README pull request when an upstream project is renamed, transferred, archived, no longer usable, loses a clear license, or no longer meets the directory scope. Explain the reason and link to supporting upstream information. Fix a canonical redirect or moved path in place rather than creating a second entry.

## Security and Licensing

Review linked instructions, scripts, dependencies, permissions, secrets handling, and network access before running them. Report vulnerabilities to the upstream maintainer through their preferred security channel; use this repository's issues for directory problems such as broken or misleading listings.

The repository's [MIT License](LICENSE) covers this repository's documentation and assets only. Each linked project remains subject to its own license and terms. Be respectful and constructive in all discussions and reviews.
