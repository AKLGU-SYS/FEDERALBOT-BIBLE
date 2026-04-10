# FED — Privacy Policy

*Last updated: April 10, 2026*

This Privacy Policy describes what data the FED Discord Bot ("the Bot") collects, how it is used, and how it is stored.

## 1. Data We Collect

### Automatically collected when the Bot joins your server:

- **Server information**: Server ID, server name, owner ID
- **Configuration data**: Settings you configure via `/fed setup` and other commands (language, roles, channels, thresholds)

### Collected during Bot operation:

- **Moderation logs**: Actions taken by the Bot (bans, kicks, mutes, warns, quarantines) including the target user ID, action type, reason, and timestamp
- **Suspicion scores**: Per-user threat scores within each server, based on behavioral analysis
- **Message metadata**: Message timestamps, channel IDs, and behavioral patterns (e.g., message frequency, duplicate detection). **We do NOT store message content permanently.**
- **Snapshot data**: Server structure snapshots (channels, roles, permissions) for rollback purposes
- **Incident reports**: Aggregated data about detected threats (raid timelines, affected users)

### Data we do NOT collect:

- Message content (analyzed in real-time, not stored)
- Direct messages
- Voice or video data
- Email addresses
- IP addresses (unless VPN/proxy detection APIs are enabled by the server administrator)
- Payment or financial information
- Personal identification documents

## 2. How We Use Data

All collected data is used exclusively to:

- Provide anti-raid and security protection to your server
- Detect and respond to threats in real-time
- Maintain moderation logs for server administrators
- Enable the undo/rollback functionality
- Generate threat reports and statistics
- Improve the Bot's detection algorithms

We do NOT:

- Sell, share, or trade any data to third parties
- Use data for advertising or marketing
- Use data for any purpose other than providing the Bot's security services
- Transfer data between servers (each server's data is isolated)

## 3. Data Storage

- All data is stored in a **local SQLite database** on a private, secured VPS
- Data is NOT stored in any cloud service or third-party database
- The VPS is protected by firewall (UFW), fail2ban, and SSH key authentication
- Data is encrypted in transit via Discord's TLS

## 4. Data Retention

- **Moderation logs**: Retained indefinitely for audit purposes, unless the server administrator requests deletion
- **Suspicion scores**: Decay over time automatically; fully purged if a user leaves the server
- **Snapshots**: Limited to 3 manual snapshots per server + automatic snapshots (older ones are automatically deleted)
- **Configuration**: Retained as long as the Bot is in the server

## 5. Data Deletion

### Automatic deletion:
- When the Bot is removed from a server, all configuration data for that server can be deleted upon request

### Manual deletion:
- Server administrators can request complete data deletion by contacting us on the support server
- Individual user scores can be reset via the `/fed score` command

### To request data deletion:
Contact **AKLGU** (@assttz) on the [FED Support Server](https://discord.gg/jWb5ArnHk6)

## 6. Third-Party Services

If enabled by the server administrator, the Bot may send limited data to third-party APIs for VPN/proxy detection:

- **proxycheck.io**: IP addresses of joining members (for VPN detection)
- **IPQualityScore**: IP addresses of joining members (for fraud scoring)
- **AbuseIPDB**: IP addresses of joining members (for reputation checks)

These services have their own privacy policies. Server administrators who enable these features are responsible for informing their members.

## 7. Children's Privacy

The Bot does not knowingly collect data from users under 13 years of age. The Bot is intended for use on Discord, which requires users to be at least 13 years old.

## 8. Your Rights

You have the right to:

- Request information about what data we hold about you
- Request deletion of your data
- Opt out of data collection by leaving servers that use the Bot

## 9. Changes to This Policy

We may update this Privacy Policy at any time. Changes will be announced on our [Discord support server](https://discord.gg/jWb5ArnHk6).

## 10. Contact

- **Developer**: AKLGU (@assttz on Discord)
- **Support Server**: https://discord.gg/jWb5ArnHk6
- **GitHub**: https://github.com/AKLGU-SYS
