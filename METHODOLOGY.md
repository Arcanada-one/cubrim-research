# Evaluation methodology

This is a reporting contract for future reviewed results, not a new benchmark.

## Declare the experiment

State the question, data class, baseline, candidate, allowed resource budget and acceptance limits before measuring. Record build/version identity, executable checksum, toolchain, platform, CPU, available memory, thread count and exact commands. Distinguish source revision from verified binary build provenance.

## Identify inputs and complete outputs

Record dataset origin, rights, byte count and checksum. Separate tuning and holdout inputs. Account for every output component required for reconstruction: headers, dictionaries, indexes, references, common bases and missing fragments. State which costs are amortized, across how many objects and under which cold/warm assumptions.

## Verify restoration

Restore every reported output and compare it byte-for-byte with the input. Missing tools, failed commands, corrupted output, timeouts and incomplete runs are failures or incomplete measurements, not zero-byte successes. Preserve error counts and avoid presenting only successful samples as the full corpus.

## Measure dimensions separately

- Full compressed/represented size, per item and aggregate by total bytes.
- Encode/decode elapsed and CPU time; input-byte throughput; first useful output where relevant.
- Peak memory with measurement scope and platform semantics specified; buffers, threads and child processes accounted for as applicable.
- Distribution size, dependencies, decoder/bootstrap cost and cold startup.
- Streaming/application latency, cold/repeat transfer cost and fallback behavior.
- Complete-system economics only when actual tariffs, workload units and integration/support assumptions are specified.

Record repetitions, warmup policy, variation and stopping rules. An unavailable metric is explicitly unmeasured. Package size, memory, throughput and latency are not interchangeable.

## Compare like with like

Name competitor versions and settings, input scope, dictionary/training assumptions and resource limits. Report per-class regressions as well as aggregate effects. Do not add improvements from unrelated experiments. A result on a declared corpus does not establish a universal ranking.

## Public evidence package

An approved report contains the question, method, rights-cleared input description, commands where publishable, result table, restoration outcome, measured trade-offs, limitations and a stable result identifier. Preserve enough information for meaningful review without embedding private code, customer data, credentials, internal logs or patent-sensitive details. Where a proprietary implementation prevents full reproduction, identify that boundary and provide an appropriate independent evaluation route rather than claiming unrestricted reproducibility.
