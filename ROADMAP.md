# Public development roadmap

Revision: 15 November 2026. This is a planned program, not a list of completed optimizations. Work within current approved resources can proceed before a funding round; larger stages depend on an agreed team and budget.

## Immediate priority

Make compression and decompression faster, reduce memory consumption and simplify distribution without losing exact restoration. Establish reproducible baselines before choosing optimizations. Keep commercial implementation private and publish reviewed knowledge separately.

## Product tracks

### Cubrim Archiver

Measure full output size, encode/decode time, CPU, peak memory and package/startup cost. Develop maximum-compression, balanced, fast and memory-limited profiles with documented trade-offs. Test on control and previously unused inputs. Extend verified platform support, including Linux x86-64 and macOS arm64, as build and restoration tests pass.

Expected outcome: a workload-specific profile that improves the required performance/resource balance while preserving exact reconstruction and backward reading.

### Cubrim Addressor

Evaluate shared data and references together with additional compression. Test larger backups, versions and synchronization workloads. Count initial base delivery, indexes, metadata, missing blocks, updates and retransmission; distinguish initial from repeated exchange. Test lookup, integrity, resumption and independent recovery.

Expected outcome: a measured complete-system advantage in a selected workload, not a smaller reference list considered in isolation.

### Cubrim Web

Develop streaming server/client compression for applications, servers, APIs and browsers. Reduce encoder/decoder cost, memory and client bootstrap size. Measure first useful output, total delivery, latency distribution, dictionary/decoder transfer and fallback behavior. Begin in controlled client/server environments; standard-browser integration is a separate stage.

Expected outcome: lower transfer volume within the application's latency/resource requirements compared with applicable baseline codecs.

## Cross-cutting program

- **Research:** primary-source discovery, testable hypotheses, private implementation experiments, recorded negative results and reviewed public findings.
- **Reliability:** exact restoration, corrupted-input handling, resource limits, compatibility fixtures, independent recovery and tested rollback.
- **Integration:** documented SDK/CLI/server contracts, repeatable deployment, versioned updates and support.
- **Adoption:** measured customer economics, paid pilot scope, annual licensing and service-provider/OEM integrations. Market scenarios are not booked revenue.
- **Industry research:** scientific datasets, intermittent/distant communications, space stations, telescopes and autonomous lunar/Mars systems. Hardware/protocol work needs dedicated requirements and partners; no flight qualification is claimed.

## Stages from the funded program's start

| Stage | Planned outcome |
|---|---|
| Next engineering cycle | Identified baseline, bottleneck profile and bounded speed/memory candidates |
| 0–6 months | Target performance profile, representative trials, rights and integration preparation |
| 6–12 months | Stable library or server module, paid deployments, updates and support |
| 12–24 months | Repeatable provider/OEM onboarding, research automation and contract expansion |
| Beyond | Additional data classes, Web integrations and dedicated industry programs |

Progress is accepted by outcome, not by a calendar label. Public results identify the tested build, workload and measurement method. An initial prototype is not a general performance guarantee.
