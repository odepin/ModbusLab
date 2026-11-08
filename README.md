# ModbusLab

> Local, deterministic Modbus device simulation for testing.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, or used. Update this status to reflect real work.

## What it is

ModbusLab is a proposed specialist software tool for Industrial automation developers, integrators, and technical educators. Communications and error-handling code is hard to validate without access to a physical controller or sensor. The intended differentiation is: Reproducible virtual device behaviors, documented register maps, and a CLI-friendly regression workflow.

## Intended users and use cases

- Read simulated sensor registers from a local client
- Test how a client handles timeouts and invalid register addresses
- Replay a scripted industrial training example

## Planned features

- Create simulated devices from declarative register maps
- Serve Modbus TCP on a local loopback test endpoint
- Script deterministic register changes and timeouts
- Emit time-stamped local test logs and replay scenarios
- Provide ready-made fictional sensor and controller configurations

## Proposed technology

Python 3.12+, pymodbus, Typer, YAML, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- Typed YAML register-map model
- Loopback-only Modbus TCP simulator
- Scenario engine with reproducible timing
- CLI and test fixtures

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Invented device maps and loopback-only network traces.`

## Data boundaries and exclusions

Connecting to, scanning, or modifying real industrial control networks or devices; no exploit or attack tooling. All public examples should use Invented device maps and loopback-only network traces.

## Known limitations / validation risks

Ensure the default binds to localhost and documentation forbids live OT deployment without independent safeguards.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Advanced integration suites, specialist protocol packs, and training materials.

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

