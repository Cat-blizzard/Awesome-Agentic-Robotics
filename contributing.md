# Contributing

Thanks for helping improve Awesome Agentic Robotics.

This list is intentionally selective. Please add resources that contribute to at least one core capability of physical agency:

- embodied memory and state maintenance
- planning, reasoning, and skill composition
- world models and world-action models
- execution verification and self-evaluation
- failure detection, attribution, and recovery
- tool use, skill calling, and robot API invocation
- long-horizon manipulation and navigation
- human-robot interaction for agentic execution
- safety, governance, and physical-risk constraints

## Adding an Entry

Please follow the existing format:

```md
- \[YYYY.M] Title [paper](https://example.com) [project](https://example.com) [code](https://example.com)
```

Use the first public release month when possible, usually the arXiv month for papers.

## Selection Criteria

Good entries should be relevant to agentic robotics, not only general robotics or generic world modeling. A paper does not need to be a complete agentic robot system, but it should clearly contribute to a component of physical agency.

Please prefer:

- peer-reviewed papers, arXiv preprints, technical reports, or well-documented open-source systems
- resources with working paper, project, or code links
- works that define a capability, benchmark, architecture, or reusable system

Please avoid:

- weakly related robotics papers with no agentic component
- pure LLM-agent papers without a robotics or embodied AI connection
- abandoned repositories or undocumented projects
- duplicate entries across multiple sections unless the cross-listing is essential

## Pull Requests

Before opening a pull request:

- check that links work
- keep entries sorted by `[YYYY.M]` in descending order within each section
- keep descriptions concise and neutral
- run `npx awesome-lint README.md`
