# Victor Condack

**Senior Backend Engineer** working with Go and C#/.NET. I build payment and core banking systems: Pix, TED, ISO 20022 messaging and the infrastructure that keeps them running.

Rio de Janeiro, Brazil · [LinkedIn](https://www.linkedin.com/in/victor-condack/)

## Selected work

- **Pix core for a Brazilian state-owned bank.** Go services integrated with the PSTI, with a measured capacity of about 50,000 transactions per second.
- **TED integrations (STR and Câmara PAG).** Go, Kafka, CockroachDB and PostgreSQL, exposed as HTTP/gRPC services on GKE and deployed through GitOps with Helm.
- **Banking-as-a-Service modernization.** Architected the migration from Python to Go: in production within two months, with about 50% higher TPS.
- **Pix ISO 20022 messaging.** pacs.008, pacs.002, pacs.004 and camt.054 over Kafka and Redis with asynchronous consumers.

Most of that code lives in private repositories. My open-source work below is public.

## Featured: [pix-in-a-box](https://github.com/victorcondackdev/pix-in-a-box)

A Pix PSP in a box, assembled from my own libraries: DICT lookup, risk decision, two-phase ledger hold, SPI transfer, signed settlement webhook, refunds and MED, plus charges flowing through a transactional outbox and Kafka to merchant webhooks. `docker compose up` runs the whole stack with Prometheus and Grafana, and CI runs five end-to-end scenarios on every push.

## Open source

| Area | Go | .NET |
| --- | --- | --- |
| Pix, boletos, CPF/CNPJ | [brpay](https://github.com/victorcondackdev/brpay) · [pix-qrcode-go](https://github.com/victorcondackdev/pix-qrcode-go) | [brpay-dotnet](https://github.com/victorcondackdev/brpay-dotnet) · [brpay-aspnetcore](https://github.com/victorcondackdev/brpay-aspnetcore) |
| API Pix and PSP tooling | [pix-cobranca-go](https://github.com/victorcondackdev/pix-cobranca-go) · [pix-psp-simulator](https://github.com/victorcondackdev/pix-psp-simulator) | |
| Messaging standards | [iso20022-pix-go](https://github.com/victorcondackdev/iso20022-pix-go) · [iso8583-go](https://github.com/victorcondackdev/iso8583-go) · [cnab-go](https://github.com/victorcondackdev/cnab-go) | [iso20022-pix-dotnet](https://github.com/victorcondackdev/iso20022-pix-dotnet) · [cnab-dotnet](https://github.com/victorcondackdev/cnab-dotnet) |
| Ledger and reconciliation | [ledger-go](https://github.com/victorcondackdev/ledger-go) · [reconcile-go](https://github.com/victorcondackdev/reconcile-go) | [ledger-dotnet](https://github.com/victorcondackdev/ledger-dotnet) |
| Reliability | [payments-service-go](https://github.com/victorcondackdev/payments-service-go) · [saga-go](https://github.com/victorcondackdev/saga-go) · [webhook-relay-go](https://github.com/victorcondackdev/webhook-relay-go) · [ratelimit-go](https://github.com/victorcondackdev/ratelimit-go) | [outbox-efcore](https://github.com/victorcondackdev/outbox-efcore) · [idempotency-aspnetcore](https://github.com/victorcondackdev/idempotency-aspnetcore) |
| Risk | [fraud-rules-go](https://github.com/victorcondackdev/fraud-rules-go) | |

The .NET libraries are parity-tested against their Go counterparts with generated vectors.

## Stack

| Area | Tools |
| --- | --- |
| Languages | Go, C#/.NET, TypeScript, Python |
| Messaging | Kafka, RabbitMQ, Redis |
| Data | PostgreSQL, CockroachDB, SQL Server |
| Infrastructure | Kubernetes (GKE), Helm, GCP, AWS, CI/CD, Prometheus |

## Shipped apps

- [Atlantic Pay](https://play.google.com/store/apps/details?id=com.atlantic.pay)
- [Urbanky Ticketeria](https://play.google.com/store/apps/details?id=com.urbanky.ticketeria)
- [Urbanky Validator](https://play.google.com/store/apps/details?id=com.urbanky.validator)
- [Urbanky Dashboard](https://play.google.com/store/apps/details?id=com.urbanky.dashboard)
