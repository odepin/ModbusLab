# ModbusLab - technical plan

**Planning document, not an implementation report.**

## Product objective

Reproducible virtual device behaviors, documented register maps, and a CLI-friendly regression workflow.

## Intended system boundary

- **Input:** Invented device maps and loopback-only network traces.
- **Processing stages:** Typed YAML register-map model; Loopback-only Modbus TCP simulator; Scenario engine with reproducible timing; CLI and test fixtures.
- **Output:** A local simulated client exercise produces the same expected trace on repeat runs.
- **Runtime / build stack (tentative):** Python 3.12+, pymodbus, Typer, YAML, pytest
- **Explicitly excluded:** Connecting to, scanning, or modifying real industrial control networks or devices; no exploit or attack tooling.

## Functional modules

- Create simulated devices from declarative register maps
- Serve Modbus TCP on a local loopback test endpoint
- Script deterministic register changes and timeouts
- Emit time-stamped local test logs and replay scenarios
- Provide ready-made fictional sensor and controller configurations

## Demonstration and acceptance cases

**Test 1:** Read simulated sensor registers from a local client

**Test 2:** Test how a client handles timeouts and invalid register addresses

**Test 3:** Replay a scripted industrial training example

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

Ensure the default binds to localhost and documentation forbids live OT deployment without independent safeguards.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
