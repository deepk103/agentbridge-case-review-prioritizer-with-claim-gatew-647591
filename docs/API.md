# API Documentation

## Endpoints
### Signal Intake
- **Description**: Collect, validate and normalize encounter summaries from EHR; attach a runId and timestamp for traceability.
- **Type**: Processing

### Discover
- **Description**: Execute discover phase for the Auto-Retrieval pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Retrieve
- **Description**: Execute retrieve phase for the Auto-Retrieval pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Plan Drafting
- **Description**: Plan Drafting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Documentation
- **Description**: Documentation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Optimization
- **Description**: Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Intervention
- **Description**: Intervention across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Orchestration
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to EHR; return response JSON for the client.
- **Type**: Processing
