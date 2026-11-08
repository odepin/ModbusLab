# ModbusLab - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A local simulated client exercise produces the same expected trace on repeat runs.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Specify register and scenario YAML | 8 | Validated schemas and fictional examples |
| 2 | Implement loopback-only simulator | 11 | Read and write basic synthetic registers |
| 3 | Add fault and timeout scenarios | 9 | Deterministic error behavior under tests |
| 4 | Create event logging and replay | 9 | Repeatable local scenario traces |
| 5 | Build CLI and example clients | 8 | End-to-end walkthrough on a laptop |
| 6 | Add tests, CI, and safeguards | 10 | No real-network access in default configuration |
| | **Total estimated** | **55** | |

## Detailed milestones

### 1. Specify register and scenario YAML (8 estimated hours)

- [ ] Deliverable: Validated schemas and fictional examples.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Implement loopback-only simulator (11 estimated hours)

- [ ] Deliverable: Read and write basic synthetic registers.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Add fault and timeout scenarios (9 estimated hours)

- [ ] Deliverable: Deterministic error behavior under tests.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Create event logging and replay (9 estimated hours)

- [ ] Deliverable: Repeatable local scenario traces.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Build CLI and example clients (8 estimated hours)

- [ ] Deliverable: End-to-end walkthrough on a laptop.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Add tests, CI, and safeguards (10 estimated hours)

- [ ] Deliverable: No real-network access in default configuration.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: Ensure the default binds to localhost and documentation forbids live OT deployment without independent safeguards.
- Commercial hypothesis (not validated): Advanced integration suites, specialist protocol packs, and training materials.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
