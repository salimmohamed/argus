# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2025-02-24

### Added

- **AI Agent**
  - Autonomous insider trading detection using Claude via AWS Bedrock
  - Agentic loop with 6 investigation tools (up to 50 iterations per case)
  - Sliding window context optimization and compressed tool responses
  - Server-side guardrails on the flagging tool (trade count, profit, confidence gates)

- **Autonomous Operation**
  - Convex cron jobs for market sync, rules detection, and AI analysis
  - Activity feed with automatic cleanup
  - Alert deduplication with 7-day window and severity escalation
  - Account and alert management utilities

- **Detection**
  - Rules-based detection with granular risk scoring
  - Expanded market coverage and suspects sorting

- **UI**
  - Suspects page with expandable evidence cards
  - Markets page header styling consistency
  - Accessibility improvements (focus states, ARIA labels)

- **Project**
  - MIT License
  - Contributing guidelines, security policy, and community files
  - GitHub issue and PR templates
  - `.env.example` for easy setup
  - Organized documentation with architecture diagrams

### Fixed

- Event slugs now resolve to condition IDs for accurate trade fetching
- Alert deduplication prevents duplicate flags within 7-day windows
- Convex functions include admin secret checks, type safety, and null handling
- Agent trigger endpoint requires authentication
- Next.js updated to 15.5.9 for security patch
- Removed redundant ARIA labels

### Changed

- Repository renamed from `colorstackwinterhack2025-argus` to `argus`
- Package renamed from `poly` to `argus`
- README rewritten for production open source use
- Images organized into `docs/images/`

### Removed

- Hackathon submission files (presentation video, slides, screenshots)
- Convex boilerplate README

## [0.1.0] - 2025-01-09

### Added

- **Core Platform**
  - Initial project setup with Next.js 15 and React 19
  - Convex serverless database with live queries for real-time updates
  - AWS Bedrock integration for Claude AI capabilities

- **Market Data**
  - Polymarket sync endpoint to fetch prediction market data
  - Automatic syncing of top political events from Polymarket
  - Support for Yes/No binary markets and multi-outcome markets

- **User Interface**
  - Argus-themed dark UI with ASCII art branding
  - Halftone eye landing page with PixelBlast visual effect
  - Markets dashboard to view monitored prediction markets
  - Responsive design with Tailwind CSS

- **Documentation**
  - Comprehensive README with setup instructions

### Fixed

- Filter out placeholder markets and extract proper candidate names
- Limit market outcomes to top 5 candidates for cleaner display
- Correct eye animation rendering on landing page

### Changed

- Migrated from SvelteKit to Next.js for better React ecosystem support

---

[Unreleased]: https://github.com/salimmohamed/argus/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/salimmohamed/argus/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/salimmohamed/argus/releases/tag/v0.1.0
