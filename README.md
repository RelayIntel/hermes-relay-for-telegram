Relay for Telegram — Hermes Agent Skill
Search, summarize, and recall your Telegram message history using AI. Built for Hermes Agent by Nous Research.

What It Does
Search across all your synced Telegram chats, groups, channels, and DMs
Summarize conversations with direct quotes and speaker attribution
Extract action items, decisions, and follow-ups
Analyze sentiment and emotional tone
Schedule automated recurring analysis with delivery to Telegram
Works with ChatGPT, Claude, and any MCP-compatible client
Quick Start
Get your API key at relayfortelegram.com
Set it as an environment variable:
export RELAY_API_KEY="rl_live_xxx"
Start asking about your Telegram messages
Installation (HermesHub)
hermes skills install github:amanning3390/hermeshub/skills/relay-for-telegram
Free Plan
10 searches per day
3 chats accessible
25 search results per query
500 messages per chat
Pro Plan
Monthly: $14.99/month
Yearly: $11.99/month (billed $143.88/year — 20% savings)
Unlimited searches, all chats, full message history
API Endpoints
Endpoint	Method	Description
/api/v1/auth/request-code	POST	Request Telegram verification code
/api/v1/auth/verify	POST	Verify code and get API key
/api/v1/search	GET	Search synced messages
/api/v1/chats	GET	List synced chats
/api/v1/chats/:id/messages	GET	Get messages from a chat
/api/v1/billing/status	GET	Check subscription status
/api/v1/billing/subscribe	POST	Subscribe to Pro
/api/v1/referrals/code	GET	Get your referral code
Privacy & Security
Read-only API access — cannot send, delete, or modify anything on Telegram
All messages encrypted at rest (AES-256-GCM)
API keys hashed (SHA-256) before storage
2FA passwords are never stored or logged
Rate-limited to 60 requests/minute per API key
Links
Homepage
Developers
Hermes Agent Skill File
Support
GitHub
Author
RelayIntel — relayfortelegram.com

License
MIT
