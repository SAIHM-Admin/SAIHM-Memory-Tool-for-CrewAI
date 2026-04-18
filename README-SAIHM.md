# SAIHM Memory Tool for CrewAI

Persistent, encrypted, cross-session memory for CrewAI agents via SAIHM (Sovereign AI Horizontal Memory) on COTI V2.

## Features

- Post-quantum encrypted memory (NIST FIPS 203/204/205)
- Cross-agent sharing via syndicate contracts (ideal for CrewAI crews)
- GDPR-compliant cryptographic erasure
- Behavioral fee discounts up to 20%

## Installation

```bash
npm install @coti-io/coti-sdk-typescript
```

## Usage with CrewAI

```python
from crewai import Agent, Task, Crew

# SAIHM-enabled agent with persistent memory
agent = Agent(
    role="Research Analyst",
    goal="Analyze data with persistent cross-session memory",
    tools=[saihm_remember, saihm_recall, saihm_forget],
    memory=True
)

# Crew with shared SAIHM syndicate contract
crew = Crew(
    agents=[agent],
    tasks=[task],
    memory=True  # Backed by SAIHM encrypted shared memory
)
```

## Network

- Mainnet: COTI V2 Helium (Chain ID: 2632500)
- RPC: `https://mainnet.coti.io/rpc`
- Fees: Write 100,000 nCOTI | Read 10,000 nCOTI

## Documentation

- [Website](https://ipfs.io/ipns/k51qzi5uqu5dkkjjdca2dl2sqilz1ahy0xdlhs0ltd691ifidqpk1b7zc4utwm/)
- [QuickStart Guide](https://ipfs.io/ipns/k51qzi5uqu5dkkjjdca2dl2sqilz1ahy0xdlhs0ltd691ifidqpk1b7zc4utwm/pdf/SAIHM_QuickStart_Top10_Agents.pdf)

## License

Apache 2.0 | Copyright 2026 SAIHM | Powered by COTI
