# Paperclip (Custom Fork for MicroForge)

![Paperclip Orchestrator](https://github.com/paperclipai/paperclip/raw/main/docs/assets/hero.png)

This is a customized fork of [Paperclip](https://github.com/paperclipai/paperclip), an orchestration layer for fully autonomous digital companies. 

## Customizations
This specific fork has been modified to support **MicroForge**, a 100% digital Micro-SaaS factory run entirely by AI agents.

### Key Changes:
- **Gemini 2.0 Flash Integration:** The native `gemini_local` adapter has been hardcoded and configured to route all agent traffic through the highly capable and fast `gemini-2.0-flash` model.
- **Quota & Rate Limit Mitigation:** By switching from OpenRouter/Hermes and other models, this fork bypasses the typical "Quota Exhausted" rate limits encountered on standard free tiers, allowing for continuous heartbeat executions of the company structure.
- **Global API Key Injection:** Safely handles environment variable injection for `GEMINI_API_KEY` during the server startup process.

## Getting Started

1. **Install Dependencies:**
   ```bash
   pnpm install
   ```

2. **Run the Server:**
   Ensure you have your `GEMINI_API_KEY` set in your environment, then run:
   ```bash
   pnpm run dev:watch
   ```

3. **Access the UI:**
   Navigate to `http://localhost:3100` to manage your agents and heartbeat runs.

---
*For the original Paperclip documentation, please refer to the [upstream repository](https://github.com/paperclipai/paperclip).*
