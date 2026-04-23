# OpenAI Codex with local LLM
Tested with llama.cpp version 8680 (15f786e65)
Testing with Codex version 0.122

# Guide
See https://unsloth.ai/docs/basics/codex

# Additional steps
After starting Codex for the first time, adjust your ~/.codex/config.toml to include `web_search = "disabled"`on the top level.

# Debugging
If you need further debugging, start llama-server with the `--verbose` flag. This will log the request as JSON. Inspect the tools payload with `cat /path/to/request_body.json | jq '.tools[].type'`.