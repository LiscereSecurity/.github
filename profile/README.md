<div align="center">

# Liscere

*Authorised is not always appropriate.*

[liscere.com](https://liscere.com/) · [Research](https://github.com/LiscereSecurity/Research) · [hello@liscere.com](mailto:hello@liscere.com)

</div>

<br>

## Mission

Industrial plants run the physical world: power, water, manufacturing, transport. The software that controls them was built for reliability, not for adversaries, and the security tools protecting them watch the network, where the asset is data.

Liscere exists to secure the layer those tools cannot see: the process itself. Know what a plant is supposed to be doing, from the plant's own behaviour, and catch the moment something acts against it.

## Why OT security is different

In IT the asset is information, and the worst case is data stolen or encrypted. In OT the asset is a physical process, and the worst case is a pump, a breaker or a furnace driven into a state that damages equipment, stops production or hurts people.

- The systems cannot simply be patched, rebooted or taken offline. Availability and safety come first.
- The controllers speak decades-old protocols with little or no authentication.
- A valid command and a malicious one look identical on the wire. The difference is not in the message; it is in whether it should have been sent.

Most defensive tooling watches the network for known-bad signatures or unusual connections. That catches the noisy attacker. It does not catch the one who uses the plant exactly as it was designed to be used, at the wrong moment.

## The threat we focus on

The most damaging OT incidents were carried out with legitimate traffic. Breakers opened by valid commands from valid consoles. Safety controllers addressed in their own protocol. Setpoints written that the drives accepted without complaint. Nothing was malformed, nothing was unauthorised, and no signature could have fired.

Liscere is built for that class of attack. By reconstructing what the process is doing at each instant, it can judge whether a control action is coherent with the state of the plant, not merely whether it is well formed.

## What it is built to catch

- A compromised engineering workstation issuing valid commands
- A malicious or mistaken insider acting outside the safe sequence
- A contractor or supply-chain foothold operating through trusted paths
- Living-off-the-land activity that never introduces malware or new connections
- Operator error that drives the process into an unsafe state

In every case the judgement is on the action and its timing, not on the identity behind it.

## How the observer works

**Reconstructs the process from traffic alone.** No P&ID, no tag list, no controller project, no asset inventory. It reads the wire and works the plant out from there.

**Runs passively and on-prem.** No agents, no active queries, nothing injected into the control network. The plant does not know it is there.

**Carries evidence for every claim.** Every statement is traceable to the traffic it came from.

**Refuses when the evidence is insufficient.** An unresolved answer is a valid result. A confident wrong one is not.

**Deterministic and reproducible.** The same capture yields the same result, every time.

**Protocols:** Modbus/TCP, S7, IEC 60870-5-104 and OPC UA today.

## Roadmap

**Now** — Reconstructing process behaviour across plant types, extending from continuous control to discrete, sequential production lines.

**Next** — The appropriateness layer at scale, on reconstructed plants: flagging a command that is valid and authorised but arrives when the process should not receive it. This is the core of what Liscere is for.

**Later** — A plant-facing view an engineer recognises in seconds and can confirm or correct, and wider protocol coverage: PROFINET, EtherNet/IP and DNP3.

## Public work

[Research](https://github.com/LiscereSecurity/Research) — technical reports and write-ups on what the observer does and what it has found.

The observer itself is developed privately. For access or a technical conversation, write to [hello@liscere.com](mailto:hello@liscere.com).

<br>

<div align="center"><sub>Liscere sp. z o.o. · Łódź, Poland</sub></div>
