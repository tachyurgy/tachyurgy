# Patrick Donahue

Senior backend engineer in Renton, Washington. Seven years on one production Rails SaaS that grew from about $4M to $13M ARR while I owned API design, PostgreSQL performance and the AWS bill. Over the past year most of my time has gone into LLM application infrastructure: streaming that survives a proxy, tool calls that fail safely, evaluation harnesses so a prompt change can be shown to have helped, and agent-driven development against real production code.

Available for contract or C2C work through Levelbrook Consulting LLC, and open to a senior IC role. Remote, US Pacific.

levelbrookteam@gmail.com · [resume (PDF)](https://levelbrook-resume.s3.amazonaws.com/levelbrook-consulting-resume.pdf) · [LinkedIn](https://www.linkedin.com/in/patrick-donahue-26947b411/) · [writing](https://consulting.levelbrook.com/writing/)

## What I would show you first

| | |
|---|---|
| [**Porchlight**](https://porchlight.ing) | A live Rails 8 product I built and run. Senior-living residents record their life stories; the app transcribes them and turns them into something staff and families can use. The repo is private, but I am happy to walk through it on a screen share. |
| [**demo.levelbrook.com**](https://demo.levelbrook.com) | Rails 8 and Hotwire. A Kanban board that morphs live across browsers with Turbo 8, per-field inline editing, and an LLM chat that streams tokens over `ActionController::Live` and SSE with a wire inspector so you can watch the frames go by. Source: [levelbrook-hotwire-demo](https://github.com/tachyurgy/levelbrook-hotwire-demo). |
| [**recourse**](https://github.com/tachyurgy/recourse) | A loan-servicing exception queue. State is folded from an append-only event log so the queue and the audit trail cannot drift, and the LLM classifier attached to it was measured against a labelled set rather than assumed to work. Live at [recourse.levelbrook.com](https://recourse.levelbrook.com). |
| [**Data Jobs Observatory**](https://datajobs.levelbrook.com) | A daily pipeline that crawls public ATS boards for remote US data jobs, models them in dbt on DuckDB, and publishes a static dashboard. Source: [datajobs-observatory](https://github.com/tachyurgy/datajobs-observatory). |
| [**linguaguessr**](https://github.com/tachyurgy/linguaguessr) | GeoGuessr for the ear. Forty languages, a Whisper-verified audio corpus I scraped and transcribed myself, served from the edge at [lingua.levelbrook.com](https://lingua.levelbrook.com). |

Upstream: [lostisland/faraday#1709](https://github.com/lostisland/faraday/pull/1709) (merged).

## Work I can talk about in detail

- Cut about $444k a year out of an S3 and Glacier bill covering 2.6 PB of objects by restructuring storage classes and lifecycle rules. The lesson was not clever engineering; it was that nobody had read the invoice line by line.
- Deployed DINOv3 on Kubernetes to compare vehicle damage photos: embed each new photo, rank it by cosine similarity against that vehicle's own history, surface the prior shot from the same angle. "Is this damage new?" became a diff.
- Built an MCP server so a support team could run data entry through Claude as a review queue, approving or rejecting proposed changes the way an engineer reviews a pull request.
- Audited a decade of Rails for N+1 queries with Prosopite, fixed hundreds across read and write paths, and attached regression specs so they could not quietly return.
- Currently rearchitecting the ingest pipeline behind roughly 3 PB of uploaded media onto Elixir, Phoenix and Ecto.

Rails is where I am fastest. Python, TypeScript and Go are in regular use, and I am not precious about the stack.
