
# .NET 8 Secure File Exchange Scaffold

This solution includes:

- `SftpWorkerService`: Downloads files via SFTP and publishes to RabbitMQ.
- `FileProcessorService`: Consumes events, validates data, calls gRPC service.
- `BusinessRulesService`: gRPC service for applying validation logic.
- `EmailNotificationService`: Sends discrepancy emails securely.
- Encrypted logging, telemetry, and retry/DLQ strategies included.
