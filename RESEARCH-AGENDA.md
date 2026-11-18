# Research agenda

This document defines questions and experimental directions. It is not a claim of a new theorem, exhaustive literature coverage or measured superiority.

## 1. Representation and compression limits

How should the complete description length of an encoding be accounted for? Study representation, modeling and coding together, including every decoder-required parameter and side-information channel. Distinguish theoretical bounds, finite-input overhead and an actual restorable format. State assumptions about the input family and decoder knowledge explicitly.

Deliverables: source-attributed reviews, mathematical statements with assumptions, counterexamples where relevant, and reproducible evaluation protocols. Proprietary realizations are not part of the public export.

## 2. Prediction, context and finite samples

When does a richer statistical model improve a practical coding result after training/adaptation, table and runtime costs? Investigate sample-size effects, sparse contexts, distribution shift and the difference between an idealized estimate and an executable implementation.

Deliverables: controlled comparisons, uncertainty/variation reporting, held-out evaluation and documented negative findings. Do not tune and report on the same evaluation slice without identifying that dependence.

## 3. Shared information and address-based transfer

How much useful shared state is available in backups, versions and repeated exchanges? What are the costs of establishing, finding, updating and recovering it? Study cold and warm states separately, including missing data, stale references, interruptions and complete restoration.

Deliverables: full storage/traffic/compute models and representative workload descriptions. A reference count alone does not establish the full-system result.

## 4. Practical performance frontiers

How do output size, encode/decode throughput, memory, startup, energy and implementation footprint trade off across data classes and platforms? Investigate bounded profiles rather than assuming one configuration is best for every constraint.

Deliverables: comparable operating points, explicit resource ceilings, repeated measurements and workload-specific recommendations derived from results.

## 5. Streaming and browser delivery

What is the total cost of transmitting and restoring an application response, including decoder and dictionary delivery? Study bounded buffers, backpressure, incremental output, cancellation, cold/repeat requests, capability negotiation and fallback.

Deliverables: end-to-end protocols and latency/traffic comparisons. Application-level support is distinct from native browser content-encoding support.

## 6. Scientific and distant-link workloads

Which classes of measurements or imagery benefit from exact representation and shared state under limited contact windows? Investigate sensor noise, onboard resources, base delivery and autonomous recovery using representative permitted data.

Deliverables: workload requirements, comparison plans and target-system experiments with domain partners. A laboratory result does not establish space-system qualification.

## Publication record

For every source, record title, authors, version/date, primary URL, access/license conditions, relevant claim, assumptions, reproduction status and relation to the question. For every result, record what was actually executed, what remained modeled and which limitations affect transfer to other workloads. The initial edition contains no completed source catalogue; adding one is an explicit next research artifact.
