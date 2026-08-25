# Contributing

Thanks for helping keep this list useful.

## What belongs here

Regulations, standards, risk frameworks, security resources, and open-source
tools that a practitioner building or auditing AI systems under regulatory
constraints would actually reach for. The list is curated, not exhaustive.

## What does not

- Vendor landing pages without substantive public content.
- Paywalled content without a meaningful public abstract.
- Abandoned projects (no activity for more than 18 months), unless they are of
  historical significance.

## How to add an entry

Open a pull request with:

1. The entry in the format `[Name](URL) - One-line description ending with a period.`
2. Placed in the correct category, in alphabetical order where practical.
3. A short justification in the PR description of why the resource is
   authoritative or practically useful.

One entry per pull request keeps review fast. Check that the link resolves and
is not already listed.

## Entry tags

Every entry is preceded by an HTML comment carrying machine-readable metadata. It is
invisible in the rendered README and exists so the list can be filtered, exported, or
re-grouped without re-parsing prose.

```markdown
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [EU AI Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) - Description.
```

| Field    | Values |
| -------- | ------ |
| `GEO`    | `Global`, `Europe`, `North America`, `Asia-Pacific`, `Latin America`, `Africa`, `Middle East` |
| `LEVEL`  | `International`, `Regional`, `National`, `State/Province` |
| `TOPIC`  | `Regulation`, `Standard`, `Principles`, `Risk Management`, `Safety`, `Security`, `Privacy`, `Evaluation`, `Transparency` |
| `STATUS` | `Binding`, `Voluntary`, `Proposed`, `Guidance` |
| `SECTOR` | `Cross-sector`, `Healthcare`, `Finance`, `Employment`, `Public Sector`, `Education`, `Critical Infrastructure`, `Autonomous Vehicles` |
| `TYPE`   | `Law`, `Framework`, `Standard`, `Database`, `Tool`, `Report`, `Policy` |

`GEO` and `LEVEL` are distinct on purpose. The Council of Europe Framework Convention is
`GEO: Europe` but `LEVEL: International` — it is a binding treaty open to non-European
states, not an EU instrument. Do not conflate "Europe" with "EU".

## The ⭐ marker

A ⭐ marks a source the maintainer opens first in an actual engagement. It is a
practitioner's shortlist, not a quality ranking of the other entries, and it is set by
the maintainer — please do not add one in a pull request.

## Quality bar

- Link to the primary source (the regulator, the standards body, the project
  repository), not to a summary of it.
- Descriptions state what the resource *is*, not why it is great.
- Disclose any affiliation. Entries you maintain are marked *(maintainer)*.

## Removals

Open an issue if an entry is dead, superseded, or no longer meets the bar.

By contributing, you agree that your contribution is released under
[CC0 1.0 Universal](LICENSE) — the public domain dedication this list uses.
