# Patrick Donahue

Senior backend engineer in Renton, Washington. Seven years on one production Rails SaaS that grew from about $4M to $13M ARR while I owned API design, PostgreSQL performance and the AWS bill. Over the past year most of my time has gone into LLM application infrastructure: streaming that survives a proxy, tool calls that fail safely, evaluation harnesses so a prompt change can be shown to have helped, and agent-driven development against real production code.

Available for contract or C2C work through Levelbrook Consulting LLC, and open to a senior IC role. Remote, US Pacific.

levelbrookteam@gmail.com · [resume (PDF)](https://levelbrook-resume.s3.amazonaws.com/levelbrook-consulting-resume.pdf) · [LinkedIn](https://www.linkedin.com/in/patrick-donahue-26947b411/) · [writing](https://consulting.levelbrook.com/writing/)

## What I would show you first

| | |
|---|---|
| [**ai_stream**](https://github.com/tachyurgy/ai_stream) | Ruby had no way to speak the Vercel AI SDK data stream protocol, so I wrote one. A Rails or Rack backend can now drive a `useChat` or `useObject` frontend directly. Zero dependencies, on [RubyGems](https://rubygems.org/gems/ai_stream). |
| [**demo.levelbrook.com**](https://demo.levelbrook.com) | Rails 8 and Hotwire. A Kanban board that morphs live across browsers with Turbo 8, per-field inline editing, and an LLM chat that streams tokens over `ActionController::Live` and SSE with a wire inspector so you can watch the frames go by. Source: [levelbrook-hotwire-demo](https://github.com/tachyurgy/levelbrook-hotwire-demo). |
| [**recourse**](https://github.com/tachyurgy/recourse) | A loan-servicing exception queue. State is folded from an append-only event log so the queue and the audit trail cannot drift, and the LLM classifier attached to it was measured against a labelled set rather than assumed to work. Live at [recourse.levelbrook.com](https://recourse.levelbrook.com). |
| [**tether**](https://github.com/tachyurgy/tether) | Static goroutine-leak analyzer built on `x/tools/go/analysis`. Run over the whole Go 1.25 standard library it found a real WaitGroup hang in the `database/sql` tests. |
| [**weave**](https://github.com/tachyurgy/weave) | Deterministic interleaving explorer for concurrent Go, roughly what Loom is for Java: stateless DFS with replay, vector-clock race detection, delta debugging. |
| [**linguaguessr**](https://github.com/tachyurgy/linguaguessr) | GeoGuessr for the ear. Forty languages, a Whisper-verified audio corpus I scraped and transcribed myself, served from the edge at [lingua.levelbrook.com](https://lingua.levelbrook.com). |

Smaller Ruby libraries: [picoglob](https://github.com/tachyurgy/picoglob) (bash globs to reusable `Regexp`) and [fzy_score](https://github.com/tachyurgy/fzy_score) (fzy/fzf scoring with matched positions).

## About the rest of the repositories here

Most of the other repos on this account are small, self-contained studies I built to think through one specific domain problem: idempotent order ingestion, a designated-giving ledger, recall-campaign scheduling, and so on. They are real code with tests, but they are sketches rather than products, and I keep them public because the reasoning in them is the point. The six above are the ones I stand behind.

## Work I can talk about in detail

- Cut about $444k a year out of an S3 and Glacier bill covering 2.6 PB of objects by restructuring storage classes and lifecycle rules. The lesson was not clever engineering; it was that nobody had read the invoice line by line.
- Deployed DINOv3 on Kubernetes to compare vehicle damage photos: embed each new photo, rank it by cosine similarity against that vehicle's own history, surface the prior shot from the same angle. "Is this damage new?" became a diff.
- Built an MCP server so a support team could run data entry through Claude as a review queue, approving or rejecting proposed changes the way an engineer reviews a pull request.
- Audited a decade of Rails for N+1 queries with Prosopite, fixed hundreds across read and write paths, and attached regression specs so they could not quietly return.
- Currently rearchitecting the ingest pipeline behind roughly 3 PB of uploaded media onto Elixir, Phoenix and Ecto.

Rails is where I am fastest. Python, TypeScript and Go are in regular use, and I am not precious about the stack.
