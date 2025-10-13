---
title: Software Supply Chain Security Technical Community Group
sidebar_label: Software Supply Chain Security
---

# Software Supply Chain Security Technical Community Group

The Software Supply Chain Security Technical Community Group (Supply Chain
Security TCG) addresses the growing importance of securing the software supply
chain. The group brings together practitioners, security professionals, and
organizations to discuss threats, best practices, tools, and standards for
supply chain security.

## Mission

The Supply Chain Security TCG aims to:

- Foster collaboration on software supply chain security challenges
- Share knowledge about supply chain threats and attack vectors
- Discuss tools and practices for supply chain security
- Coordinate with industry standards and frameworks (SLSA, SBOM, etc.)
- Promote adoption of supply chain security best practices
- Support development of cloud native supply chain security solutions

## Focus Areas

The Supply Chain Security TCG discusses topics including:

- **Software Bill of Materials (SBOM)** - Generation, management, and
  consumption of SBOMs
- **Provenance and Attestation** - Build provenance, artifact signing, and
  verification
- **SLSA Framework** - Supply-chain Levels for Software Artifacts adoption and
  implementation
- **Dependency Management** - Securing and managing software dependencies
- **Build Security** - Secure build environments, reproducible builds
- **Artifact Verification** - Signature verification, policy enforcement
- **Vulnerability Management** - Scanning, tracking, and remediating supply
  chain vulnerabilities
- **Policy and Compliance** - Supply chain security policies and regulatory
  requirements
- **Tooling Integration** - Integrating supply chain security into CI/CD
  pipelines
- **Incident Response** - Responding to supply chain attacks and compromises

## Meetings

### Regular Meetings

- **Schedule**: Check the [CNCF Public Calendar](https://www.cncf.io/calendar/)
  for current meeting times
- **Format**: Virtual meetings via Zoom
- **Recordings**: Available on the
  [CNCF YouTube Channel](https://www.youtube.com/c/cloudnativefdn)

### Meeting Resources

| Resource       | Link                                                  |
| -------------- | ----------------------------------------------------- |
| Meeting Notes  | [GitHub Repository or Google Docs]                    |
| Meeting Agenda | Check Slack channel for agenda items                  |
| Calendar       | [CNCF Public Calendar](https://www.cncf.io/calendar/) |

## Communication Channels

### Slack

- **Primary Channel**: `#tcg-supply-chain-security` on
  [CNCF Slack](https://cloud-native.slack.com)
- **Related Channels**:
  - `#tag-security-supply-chain` - TAG Security supply chain working group
  - `#sig-security` - Broader security discussions
- **Join**: Get an invite at [slack.cncf.io](https://slack.cncf.io)

### Mailing List

- **List**: Check the [CNCF TOC repository](https://github.com/cncf/toc) or
  Slack for mailing list information
- **Purpose**: Official TCG communications and announcements

### GitHub

- **Discussions**: Primary discussions happen in Slack and meetings
- **Resources**: Relevant materials may be shared via GitHub repositories

## Leadership

As a Technical Community Group, the Supply Chain Security TCG is organized by
community volunteers who facilitate meetings and coordinate activities.
Leadership is informal and community-driven.

## Current Activities

The Supply Chain Security TCG facilitates:

- **Knowledge Sharing** - Presentations on supply chain security topics
- **Threat Analysis** - Discussing current and emerging supply chain threats
- **Tool Evaluations** - Community reviews of supply chain security tools
- **Best Practice Development** - Documenting patterns for securing the supply
  chain
- **Standards Alignment** - Coordinating with industry standards like SLSA, SBOM
  formats
- **Incident Learning** - Analyzing supply chain security incidents
- **Community Building** - Connecting practitioners across organizations

## Relationship with TAG Security

The Supply Chain Security TCG works closely with
[TAG Security](../../tags/security-and-compliance/index.md), particularly with
TAG Security's supply chain security initiatives:

- **Coordination** - Regular coordination on supply chain security topics
- **Complementary Focus** - TCG provides discussion forum; TAG produces formal
  deliverables
- **Shared Participation** - Many participants are active in both groups
- **Information Flow** - Insights from TCG discussions inform TAG Security work

## Getting Involved

### Join the Community

1. Join the Supply Chain Security TCG channel on
   [CNCF Slack](https://slack.cncf.io)
2. Subscribe to the mailing list (if available)
3. Attend TCG meetings (check the
   [CNCF calendar](https://www.cncf.io/calendar/))
4. Introduce yourself and share your supply chain security interests

### Participate

There are many ways to participate:

- **Share your experience** with supply chain security challenges
- **Discuss incidents** and lessons learned (anonymized as needed)
- **Present tools** and solutions you're using
- **Ask questions** and learn from other practitioners
- **Contribute** to best practice documentation
- **Connect** with others working on similar problems
- **Organize** initiatives within the group

### Present at a Meeting

To present at a Supply Chain Security TCG meeting:

1. Propose your topic in the Slack channel
2. Coordinate with the meeting organizers on scheduling
3. Prepare your presentation
4. Share your knowledge with the community

## Key Topics of Interest

### SBOM Generation and Management

Understanding different SBOM formats (SPDX, CycloneDX), generating SBOMs for
cloud native applications, and using SBOMs for security analysis.

### SLSA Adoption

Implementing the SLSA (Supply-chain Levels for Software Artifacts) framework in
cloud native environments.

### Signing and Verification

Using tools like Sigstore, Cosign, and others to sign and verify artifacts
throughout the supply chain.

### Build Security

Securing build environments, implementing hermetic builds, and ensuring build
reproducibility.

## Related CNCF Projects

CNCF projects relevant to supply chain security:

- **Sigstore** - Software signing and transparency
- **in-toto** - Supply chain security framework
- **SPIFFE/SPIRE** - Identity and authentication
- **Falco** - Runtime security and threat detection
- **OPA** - Policy-as-code for security controls
- And many others in the [CNCF Landscape](https://landscape.cncf.io/)

## External Resources

### Industry Standards

- **SLSA** - [slsa.dev](https://slsa.dev) - Supply-chain Levels for Software
  Artifacts
- **SBOM** - [ntia.gov](https://www.ntia.gov/sbom) - Software Bill of Materials
- **SSDF** - [NIST SSDF](https://csrc.nist.gov/projects/ssdf) - Secure Software
  Development Framework

### Related Initiatives

- **OpenSSF** - [openssf.org](https://openssf.org) - Open Source Security
  Foundation
- **CISA** - [cisa.gov](https://www.cisa.gov) - Cybersecurity and Infrastructure
  Security Agency

## Resources

| Resource                                                    | Description                                    |
| ----------------------------------------------------------- | ---------------------------------------------- |
| [TAG Security](../../tags/security-and-compliance/index.md) | Related CNCF TAG with supply chain initiatives |
| [CNCF TOC Repository](https://github.com/cncf/toc)          | Main repository for CNCF governance            |
| [CNCF Slack](https://slack.cncf.io)                         | Join the Supply Chain Security TCG channel     |
| [CNCF Calendar](https://www.cncf.io/calendar/)              | Find meeting times                             |
| [CNCF Security TAG](https://github.com/cncf/tag-security)   | TAG Security repository                        |

## Future Direction

The Supply Chain Security TCG serves as a forum for community discussion and
coordination on this critical topic. As the community grows and matures, it may
evolve to take on additional responsibilities or develop formal deliverables in
coordination with TAG Security.
