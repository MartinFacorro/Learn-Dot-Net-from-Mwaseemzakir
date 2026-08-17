# Databases & Data Access

A decision guide for picking a database and a data-access approach for your .NET app — not just links, but *when to use what*. For the concrete NuGet packages, see [Libraries](./libraries.md).

## Choosing a database

| Database | Best for | .NET access |
| --- | --- | --- |
| [SQL Server](https://www.microsoft.com/en-us/sql-server/) | Default for most enterprise .NET apps; deep tooling and EF Core support. | EF Core / Dapper |
| [PostgreSQL](https://www.postgresql.org/) | Modern open-source default; great features, JSON, and cost. | EF Core ([Npgsql](https://www.npgsql.org/)) |
| [SQLite](https://www.sqlite.org/) | Local, embedded, desktop/mobile, and tests — zero server. | EF Core / Microsoft.Data.Sqlite |
| [MySQL / MariaDB](https://www.mysql.com/) | Existing MySQL estates and LAMP-style hosting. | EF Core (Pomelo) |
| [Azure Cosmos DB](https://learn.microsoft.com/en-us/azure/cosmos-db/) | Globally distributed, low-latency NoSQL on Azure. | Cosmos SDK / EF Core |
| [MongoDB](https://www.mongodb.com/) | Flexible document model and rapid iteration. | MongoDB.Driver |
| [Redis](https://redis.io/) | Caching, sessions, and real-time data — not a primary store. | StackExchange.Redis |

## Choosing a data-access approach

| Approach | Use when |
| --- | --- |
| [EF Core](https://learn.microsoft.com/en-us/ef/core/) | You want a full ORM: change tracking, LINQ, and migrations. The default for most apps. |
| [Dapper](https://github.com/DapperLib/Dapper) | You need raw speed and full control over SQL with minimal overhead. |
| [Hybrid (EF Core + Dapper)](https://learn.microsoft.com/en-us/ef/core/) | EF Core for writes and most reads; drop to Dapper for hot, complex queries. |

## Learn

1. [EF Core Documentation](https://learn.microsoft.com/en-us/ef/core/)

	The official, comprehensive guide to Entity Framework Core — modeling, querying, and saving data.

2. [EF Core Database Providers](https://learn.microsoft.com/en-us/ef/core/providers/)

	The full list of supported databases and the NuGet provider for each.

3. [EF Core Migrations](https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/)

	How to evolve your database schema safely over time with code-based migrations.

4. [Dapper](https://github.com/DapperLib/Dapper)

	The micro-ORM repo and docs — fast, simple SQL mapping when you want control.
