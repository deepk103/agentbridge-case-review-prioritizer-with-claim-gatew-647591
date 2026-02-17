# Architecture Documentation

## Overview
This Auto-Retrieval implements Case Review Prioritizer with Claim Gateway for Healthcare & Life Sciences use cases.

## Components
1. **Signal Intake**: Collect, validate and normalize encounter summaries from EHR; attach a runId and timestamp for traceability.
2. **Discover**: Execute discover phase for the Auto-Retrieval pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Retrieve**: Execute retrieve phase for the Auto-Retrieval pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Plan Drafting**: Plan Drafting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Documentation**: Documentation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Optimization**: Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Intervention**: Intervention across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Orchestration**: Assemble final payload with status, artifacts, KPIs and audit trail; store to EHR; return response JSON for the client.

## Data Flow
- Input: Signal Intake
- Processing: 8 sequential steps
- Output: Orchestration
