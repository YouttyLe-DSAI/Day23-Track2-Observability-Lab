# Bonus Challenge Reflection

## Provocation 1: Attach telemetry to a previous day's lab

### What surprised you?
I was surprised by how easy it was to integrate metrics from completely different lab environments into a single OpenTelemetry-based stack. Using stub scripts to simulate metrics for Day 19 (Qdrant) and Day 20 (llama.cpp) allowed me to visualize the entire AI lifecycle — from vector retrieval to model inference — in a single Grafana dashboard without having to run all the underlying heavy infrastructure simultaneously.

### If you had 8 more hours, what would you build next?
If I had more time, I would implement **automated alerting based on cross-day correlations**. For example, I would create an alert that fires if the vector store (Day 19) latency increases simultaneously with the model serving (Day 20) error rate, helping to identify if a specific batch of data or model update caused a systemic failure across the entire RAG pipeline.
