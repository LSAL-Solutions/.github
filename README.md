# .github

LSAL-Solutions' organization defaults. GitHub uses a file here for every repository in the organization that has no
file of its own of that kind ([default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)).

| File | What |
|---|---|
| `pull_request_template.md` | every pull request's description: Summary, Changes, **Depends on**, **Followed by**, Deploy, Testing |

**Depends on** and **Followed by** say a pull request's merge order across the repositories, one `owner/repo#number`
per line. The PR reviewer (the agent harness's `worker`) reads them to order merges, and holds a pull request until
every pull request under its **Depends on** has merged.

This repository is public, as GitHub requires for organization defaults: it holds templates only.
