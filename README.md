# ask

A minimal Bash CLI that sends prompts to any OpenAI-compatible chat completions API.

Built as a small, hackable tool. Only two dependencies: `curl` and `jq`.

## Requirements

- Bash 3.2+ (default on macOS and Linux)
- `curl`
- `jq`

On macOS: `brew install jq`
On Debian/Ubuntu: `sudo apt install jq curl`

## Configuration

`ask` reads three environment variables:

| Variable       | Description                                         |
|----------------|-----------------------------------------------------|
| `ASK_API_URL`  | Full chat completions endpoint URL                  |
| `ASK_MODEL`    | Model name to use                                   |
| `ASK_API_KEY`  | Bearer token for the provider                       |
