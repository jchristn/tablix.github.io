# Tablix Marketing Messaging Foundation

## One-Sentence Positioning

Tablix is open-source database chat and agent infrastructure that gives models the schema, context, and guardrails they need to answer from real query results instead of guessed SQL.

## The Wedge

Every "AI + SQL" workflow tends to fall into one of two failure modes:

1. The ungrounded chat loop. It writes confident SQL against a schema it half-remembers, invents column names, and reports row counts that do not exist.
2. The read-only toy. It generates SQL, then tells the user to run it. The loop never closes, so nothing is verified.

Tablix closes the loop and keeps the loop safe. The agent discovers, the agent asks, Tablix validates and executes, and the answer comes back with the SQL and row count attached.

## Three Pillars

| Pillar | What it means | Proof point |
| --- | --- | --- |
| Understanding | Schema geometry plus durable, human-editable context about what the data means | Crawled tables, keys, indexes, database- and table-scope context, context quality scoring, inferred relationship candidates labeled separately |
| Execution | The agent runs the query, not the user | `tablix_execute_query`, statement-type allowlists, single-statement enforcement |
| Verification | Every answer carries its receipts | Verification envelope: `verified`, `partial`, `blocked`, or `ambiguous`, plus SQL, row count, and evidence |

## Voice

Technical, specific, unhurried.

Avoid broad launch language such as "revolutionize" or "unlock the power of." Show a command, payload, contract, or concrete workflow before using an adjective. Every claim should be something a skeptical staff engineer could verify in ten minutes with `docker compose up`.

Be clear about product maturity without making alpha status the first thing a visitor sees. Put limits where they help an evaluator make a deployment decision.
