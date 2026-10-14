# Command Line Interface — TOBII_STREAM_ENGINE

**Upstream:** https://github.com/Tobii/tobii-stream-engine

## Anticloud CLI

```bash
# Install
pip install anticloud-tobii-stream-engine

# Run offline with PAX inference
anticloud-tobii-stream-engine --offline --pax-local

# Run with AIOSS logging
anticloud-tobii-stream-engine --aioss-log ./ledger.jsonl

# Single binary (after build)
./tobii_stream_engine --config config.yaml
```

## Options

| Flag | Description |
| --- | --- |
| `--offline` | Disable all network calls |
| `--pax-local` | Use local PAX inference at 127.0.0.1:11434 |
| `--aioss-log PATH` | Write AIOSS audit chain to PATH |
| `--encrypt` | Enable AES-256 at rest for output files |
| `--gpu` | Force GPU inference |
| `--cpu` | Force CPU inference |
| `--config PATH` | Load configuration from YAML file |
