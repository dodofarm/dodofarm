## Hi! 🦤

I love working on open source projects as well as open sourcing my own projects.
Beyond my day job I'm currently working on [Feuerstein](https://github.com/feuerstein-org), essentially a setup where I'm building the data pipelines ([foerderturm repo](https://github.com/feuerstein-org/foerderturm)) and infrastructure ([bergschacht CDK repo](https://github.com/feuerstein-org/bergschacht-public)) for trading research which is essentially fully open source.

I also spent quite a bit of time recently looking into codegen, OpenAPI and Smithy, while writing SDKs for some financial APIs I realized that a lot of the logic like pagination and rate limiting (see my Redis based ratelimiter [here](https://github.com/feuerstein-org/steindamm)) can be shared so I created an API client SDK framework - [spitzeisen](https://github.com/feuerstein-org/spitzeisen). To eventually be able to generate code from just an OpenAPI spec or a Smithy model I'm hoping to use [smithy-translate](https://github.com/disneystreaming/smithy-translate) but for now we need to finalize [OpenAPI 3.1 support](https://github.com/disneystreaming/smithy-translate/issues/306).

My SDKs:

 - [massive-api](https://github.com/feuerstein-org/massive-api) - Massive.com API, I've added a few API endpoints I needed but more to follow
 - [eodhd-py](https://github.com/feuerstein-org/eodhd-py) - Async Python client for EODHD financial data APIs
 - [spitzeisen](https://github.com/feuerstein-org/spitzeisen) - Python framework for API clients with shared retries, pagination, rate limiting and response validation
 - [steindamm](https://github.com/feuerstein-org/steindamm) - Rate limiters with local and Redis backends (used by every SDK)


Feuerstein - financial data pipelines/processing:

 - [foerderturm](https://github.com/feuerstein-org/foerderturm-public) - Market data ingestion with Dagster
 - [bergschacht](https://github.com/feuerstein-org/bergschacht-public) - AWS infrastructure, pipelines and data-lake schemas
 - [bergtalzug](https://github.com/feuerstein-org/bergtalzug) - Python ETL pipelines with queues and workers
 - [seilbahn](https://github.com/feuerstein-org/seilbahn-public) - GitHub Actions workflows
 - [bergschacht-custom-resources](https://github.com/feuerstein-org/bergschacht-custom-resources-public) - CDK custom resources e.g. for managing S3 Tables

Languages I enjoy the most:

 - Python🐍 for automation and data processing/collection with DuckDB and polars
 - Rust🦀 for anything where performance matters - e.g. all the trading strategies I have are written in Rust (sadly can't be open sourced)
 - TypeScript(CDK) for infrastructure
 - Scala - a new language I got to use just recently but find very elegant
 - Java - I don't really interact with it outside of work but when I do it's very welcome
