# MuzixDiagSys

## 2026-08-19 Engineering Intelligence Platform

The additive Engineering Intelligence Platform integrates ten cross-domain engineering capabilities without removing existing simulator features or creating parallel implementations of established solvers: **Whole-Vehicle Consequence Engine, Zonal E/E Architecture Synthesizer, Vehicle Software Service-Graph Simulator, End-to-End Timebase Laboratory, Cross-Domain Conservation Auditor, Parameter Identifiability & Sloppiness Laboratory, Signal-Lineage / Calibration Provenance, Simulation Causality Microscope, Computational Reproducibility Capsules, and Cross-Layer Requirement Propagation**. Consequence and causality analysis share one engineering dependency graph; zonal synthesis extends the canonical `EeArchitectureSynthesizer`; conservation extends `ConservationGovernor`; and identifiability reuses the established SVD/rank/correlation path.

```bash
./build/full/muzixdiagsys_advanced_platform engineering-intelligence capabilities
./build/full/muzixdiagsys_advanced_platform engineering-intelligence self-test build/engineering-intelligence/self-test build/engineering-intelligence/self-test.json
./build/full/muzixdiagsys_advanced_platform engineering-intelligence whole-vehicle-consequence-engine request.json result.json
```

See **[`docs/ENGINEERING_INTELLIGENCE_PLATFORM.md`](docs/ENGINEERING_INTELLIGENCE_PLATFORM.md)**, User Manual Chapter 91, and the Engineering Intelligence section of `docs/MUZIXDIAGSYS_TUTORIAL_AND_EXACT_COMMAND_GUIDE.md`. The 2026-08-19 PTY regression hardening also replaces split-buffer command/focus synchronization with ordered continuous-buffer matching; this corrects a test race without changing terminal UI behavior.


## 2026-08-14 V20.1.2 Integrated Terminal Engineering Cockpit

V20.1.2 now extends the Unified Engineering Workspace with an integrated terminal engineering cockpit while preserving every existing backend and command family. The terminal adds high-resolution Unicode telemetry sparklines, a correlated event timeline, time-travel controls, causal inspection, experiment and job cockpits, notifications, analytical lower-pane tabs, a hierarchical subsystem navigator, parameter and inline-documentation inspectors, UI undo/redo, motorsport pit-wall instrumentation, terminal track mapping, a friction-circle view, runtime-profiler dashboards, and compact uncertainty rendering. These views project the existing authoritative `TelemetryWorkbench`, `SynchronizedTimeCursor`, `CausalDifferenceExplorer`, `ExperimentMatrix`, Mission Control `JobManager`, `ContextGraph`, `ExperienceManager`, run-comparison store, profiler, and command-help registry rather than creating duplicate state or parallel services. Every new backend-facing UI surface has a canonical `ui ...` route in `InteractiveShell`. See Chapters 82–84 of the User Manual and `docs/ENGINEERING_UI_PLATFORM.md`.

## 2026-08-12 V19 help, diagnostics, and documentation overhaul

V19 unifies command help, nested completion descriptions, semantic validation, raw runtime-error guidance, browser Problems diagnostics, and the User Manual around the canonical command registry. Use `help <command-or-subcommand>` for detailed behavior and syntax, `help search <term>` for discovery, `help errors [CODE]` for meaning/cause/recovery/examples, `ui semantic <command-line>` for pre-execution validation, and `ui preview <command-line>` before consequential state changes. Existing commands, aliases, simulator features, V18 stability work, and V17 solver/runtime capabilities remain available. See Chapter 80 of the User Manual.


## 2026-08-12 V17 simulation-core scalability and reuse

V17 extends existing services with JFNK; sparse-AD coloring; Jacobian/factorization reuse; block/Schwarz/AMG preconditioning; waveform relaxation; power bonds; deterministic heterogeneous scheduling; error-controlled mixed precision; reusable HIP graphs/persistent memory; and `SemanticResultCache`-backed incremental simulation. Existing solver/coupling/compute/task/cache paths remain available; see Chapter 79 and the component documents.

## 2026-08-10 Frontier Professional Integration

The additive Frontier Professional Integration implements ten previously absent professional/research interfaces without removing existing simulator features: **OPC UA/AAS; physical DIL + OpenXR; real SocketCAN/PCAN/Kvaser plus vendor-plugin hardware I/O; real ns-3 external packet federation with a supplied ns-3 bridge; four executable Jupyter labs; Prometheus metrics/HTTP export; Sigstore/in-toto provenance; HMC/NUTS + adaptive MLMC; delay-and-sum/MVDR beamforming + FxLMS ANC; and FedProx/Krum/asynchronous/differentially-private/X25519-secure extensions to the existing fleet federated-learning platform**.

Build the focused operator surface with `--target muzixdiagsys_frontier_professional frontier_professional_integration_tests`. Run `muzixdiagsys_frontier_professional capabilities` to distinguish optional native runtimes from deterministic/reference paths. See **[`docs/FRONTIER_PROFESSIONAL_INTEGRATION.md`](docs/FRONTIER_PROFESSIONAL_INTEGRATION.md)** and Chapter 73 of the User Manual. The release evidence is recorded in **[`FRONTIER_PROFESSIONAL_INTEGRATION_IMPLEMENTATION_REPORT_2026-08-10.md`](FRONTIER_PROFESSIONAL_INTEGRATION_IMPLEMENTATION_REPORT_2026-08-10.md)** and **[`FRONTIER_PROFESSIONAL_INTEGRATION_VALIDATION_2026-08-10.txt`](FRONTIER_PROFESSIONAL_INTEGRATION_VALIDATION_2026-08-10.txt)**.


## 2026-08-08 robustness and refactor qualification

A preservation-first maintenance pass hardens workspace persistence, bounded UI queries, probabilistic model checking, and Python RL adapter invariants without removing any existing simulator feature, command, alias, option, motorsports platform, or build option. The complete Release `muzixdiagsys` target builds and links successfully after the changes. See **[`DEBUG_REFACTOR_REPORT_2026-08-08_V3.md`](DEBUG_REFACTOR_REPORT_2026-08-08_V3.md)** and **[`DEBUG_REFACTOR_VALIDATION_2026-08-08_V3.txt`](DEBUG_REFACTOR_VALIDATION_2026-08-08_V3.txt)**.

## 2026-08-08 Frontier Next platform

The additive `frontier-next` platform adds sixteen executable engineering domains and sixteen dedicated CLI aliases: wireless PHY/coexistence, secure UWB/Bluetooth ranging, complex structured robustness, stochastic subspace identification, distributed protocol verification, automotive static verification, PETSc/SUNDIALS/HYPRE solver adapters, distributed GPU communication with optional NCCL, ADIOS2 streaming, CGNS/XDMF/Exodus mesh interchange, IBIS/AMI/Touchstone SI, R1234yf/R744 heat-pump analysis, NDE/metrology, model maturity/validity, scenario-space coverage, and probabilistic model-form uncertainty. Existing simulator, motorsports, diagnostic, and earlier frontier command families remain available.

```bash
./build/full/muzixdiagsys_advanced_platform frontier-next capabilities
./build/full/muzixdiagsys_advanced_platform frontier-next self-test build/frontier-next/self-test-work build/frontier-next/self-test.json
./build/full/muzixdiagsys_advanced_platform wireless-phy run examples/frontier_next/wireless_phy.json build/frontier-next/wireless.json
```

See `docs/FRONTIER_NEXT_PLATFORM.md`, Chapter 68 of the user manual, and `examples/frontier_next/`.

The additive `frontier-integration` command family adds fourteen fully executable integration and assurance domains: DDS-XRCE/Zenoh edge federation; AES-256-GCM MACsec link protection; automotive EMC sweep/immunity qualification; distributed-RLGC harness SI/PI; continuous-time bounded-real H-infinity certification with structured-real uncertainty margins; ARX/DMD/ERA system identification; Lean/Coq/Isabelle proof-artifact bridging; persistent OSLC/SACM lifecycle assurance; cycle-accurate RTL with optional real Verilator compilation/execution; SQLite engineering data queries with unit metadata; adhesive/paint/weld/stamping/resin-infusion manufacturing physics; Jacobian/covariance cross-domain error propagation; globally optimized multifidelity scheduling; and Bayesian autonomous experiment planning. Existing simulator, motorsports, CLI, frontier-expansion, and frontier-systems functionality remains available.

```bash
./build/full/muzixdiagsys_advanced_platform frontier-integration capabilities
./build/full/muzixdiagsys_advanced_platform frontier-integration self-test build/frontier-integration/self-test
```

See `docs/FRONTIER_INTEGRATION_PLATFORM.md` and `examples/frontier_integration/` for schemas and runnable requests.


## 2026-08-07 Frontier systems platform

The additive `frontier-systems` command family adds twelve fully executable engineering domains: automotive TSN timing/conformance analysis with BMCA-style clock qualification, Qbv schedule synthesis, preemption, policing/shaping, redundant-route and queue/latency certificates; native Zarr/HDF5/NetCDF scientific data interchange; VTK/Gmsh/native-topology VTKHDF mesh/field interchange plus in-situ reduction; external OpenFOAM/SU2/CalculiX/Code_Aster/Elmer case federation; portable serial/OpenMP/optional-Kokkos numerical kernels; MPI-RMA/CUDA-aware PGAS qualification; common-Lyapunov robust-control synthesis; safety-critical MPC and moving-horizon estimation; reverse-mode and optional Enzyme compiler-native automatic differentiation; calibrated/flow-capable event-camera sensing; raw FMCW radar ADC synthesis with multipath/interference and range-Doppler-angle processing; and semantic unit/frame/time/conservation contracts with uncertainty, numerical-error, differentiability, interpolation and extrapolation policies. All existing simulator and CLI features remain available.

```bash
./build/full/muzixdiagsys_advanced_platform frontier-systems capabilities
./build/full/muzixdiagsys_advanced_platform frontier-systems self-test build/frontier-systems-self-test
```

See [`docs/FRONTIER_SYSTEMS_PLATFORM.md`](docs/FRONTIER_SYSTEMS_PLATFORM.md), Chapters 65-66 of the user manual, and [`examples/frontier_systems/`](examples/frontier_systems/).

## 2026-08-07 Frontier expansion platform

The additive `frontier-expansion` command family adds fourteen production domains to `aesim_advanced`: constrained safe policy learning, CMP-oriented capture/replay, normalized traffic-participant semantics, a versioned SysML v2 repository, checksummed compressed scientific streaming, MPI-4-aware transport, independently qualified internal/external linear solvers, SENT/PSI5/DSI3/CXPI physical-layer simulation, MaterialX/glTF material round trips, host plus optional HIP particle multiphysics, lubricant chemistry/condition monitoring, tire acoustic/uniformity analysis, HAZOP/bow-tie barrier assurance, and SPDX/VEX/SARIF-oriented software-supply-chain evidence. All prior CLI commands and simulator features remain available.

```bash
./build/full/muzixdiagsys_advanced_platform frontier-expansion capabilities
./build/full/muzixdiagsys_advanced_platform frontier-expansion self-test build/frontier-expansion-self-test
```

See [`docs/FRONTIER_EXPANSION_PLATFORM.md`](docs/FRONTIER_EXPANSION_PLATFORM.md) and the executable request set in [`examples/frontier_expansion/`](examples/frontier_expansion/).


## 2026-08-07 Frontier runtime, positioning, and sensing expansion

The additive `frontier-runtime` advanced-platform family implements ULFM-resilient distributed execution, strict error-bounded ZFP/SZ3 checkpoint profiles, file-backed out-of-core arrays, NUMA/GPU-aware hardware placement, formal binary64 forward-error certificates, Lie-group and variational integration, Radau IIA/Rosenbrock-W/IMEX stiff solvers, a full carrier-phase GNSS factor graph (Standalone/PPP/RTK/PPP-RTK with dual-frequency, Doppler, ambiguity fixing, IMU/wheel/map factors), SPAD LiDAR, coherent FMCW LiDAR, and radar micro-Doppler/polarimetry. The permanent command line and all prior features remain available. See [`docs/FRONTIER_RUNTIME_SENSING_PLATFORM.md`](docs/FRONTIER_RUNTIME_SENSING_PLATFORM.md) and Chapter 64 of the user manual.

```bash
./build/full/muzixdiagsys_advanced_platform frontier-runtime capabilities
./build/full/muzixdiagsys_advanced_platform frontier-runtime self-test build/frontier-self-test
```

## Comprehensive user manual

The complete operator and engineering reference is available as editable Markdown at **[`docs/MUZIXDIAGSYS_USER_MANUAL.md`](docs/MUZIXDIAGSYS_USER_MANUAL.md)** and as a typeset PDF at **[`docs/MUZIXDIAGSYS_USER_MANUAL.pdf`](docs/MUZIXDIAGSYS_USER_MANUAL.pdf)**. The 2026-07-28 revision integrates the scientific-fidelity and generalized scientific-simulation platforms, the complete Formula One multiphysics, optimization, and real-time platform, the predictive-fidelity platform, the Formula One industrial and regulatory systems, six-module IndyCar, the 40-domain NASCAR platform, and the additive twelve-domain NASCAR integrated-fidelity platform. The newest IndyCar module adds integrated multi-rate co-simulation, telemetry assimilation/calibration, 22-DOF multibody dynamics, thermo-viscoelastic tires, unsteady aeroelastic aerodynamics, closed-loop ECU/hybrid control, radio and timing uncertainty, multi-car pit-lane events, occupant biomechanics, and unified uncertainty/model-validity supervision. The broader IndyCar surface also retains its 2028 power-unit, hybrid, driveline, brake, track/weather, full-field racecraft, incident, pit-vision, appeals, and Month-of-May systems. The NASCAR integrated module adds deterministic co-simulation, telemetry assimilation/calibration, unified uncertainty and validity supervision, a 28-DOF flexible Next Gen plant, detailed asymmetric tires, unsteady aeroelastic wakes and flaps, closed-loop ECU/driveline control, cranktrain/oil/fuel/thermal systems, shared pit road, occupant heat/egress, scanned pavement, and spray optics. It also documents the dedicated `aesim_nascar` library, the ten-domain NASCAR next-generation engineering and operations expansion, corrected NASCAR semantics, and the complete current vehicle, diagnostics, interoperability, safety, qualification, multiphysics, autonomy, manufacturing, infrastructure, and digital-twin feature set.

Use **[`docs/DOCUMENTATION_INDEX.md`](docs/DOCUMENTATION_INDEX.md)** to locate the authoritative manual, tutorial, platform references, examples, implementation reports, and validation records. Regenerate the PDF after editing the Markdown source with `./tools/generate_user_manual_pdf.sh`. The generator preserves the established letter-size layout and wraps long command examples within the printable area.

## 2026-08-01 CTest Python runtime and source-package correction

The advanced Python runtime qualification now always exercises the dependency-free C++ JSON learning-environment backend. Optional Gymnasium/PettingZoo and Arrow/Parquet adapters are tested when installed instead of causing the entire CTest case to be skipped. Dependency-complete CI can require every optional adapter with `-DMUZIXDIAGSYS_REQUIRE_OPTIONAL_PYTHON_RUNTIME=ON`.

The deterministic source-package regression now enforces independent compressed-size, expanded-size, member-count, and largest-member budgets. Existing generated-output exclusion, executable-mode preservation, path-traversal rejection, symlink rejection, and deterministic archive checks remain active. See **[`CTEST_RUNTIME_SOURCE_PACKAGE_FIX_REPORT_2026-08-01.md`](CTEST_RUNTIME_SOURCE_PACKAGE_FIX_REPORT_2026-08-01.md)** and **[`CTEST_RUNTIME_SOURCE_PACKAGE_FIX_VALIDATION_2026-08-01.txt`](CTEST_RUNTIME_SOURCE_PACKAGE_FIX_VALIDATION_2026-08-01.txt)**.

## 2026-07-30 Global Mathematical Assurance Platform

The shared `aesim_core` library now exports result-level mathematical assurance:

```cpp
#include "aesim/core/mathematical_assurance.hpp"
```

The additive platform implements classified automatic error budgets, condition-aware precision escalation through binary64, extended, decimal50, and decimal100 tiers, exact dyadic sums/dot products/polynomial references with explicit nearest-even binary64 rounding, Richardson/GCI convergence analysis, executable ODE and Poisson manufactured-solution tests, independent derivative certification, KKT and Hessian optimization certification, cross-solver consensus, deterministic property-based testing with counterexample shrinking, and SHA-256-sealed per-result mathematical evidence. Existing numerical solvers and every simulator feature remain available.

Focused validation:

```bash
cmake -S . -B build/math-assurance -G Ninja \
  -DCMAKE_BUILD_TYPE=RelWithDebInfo -DBUILD_TESTING=ON
cmake --build build/math-assurance --target mathematical_assurance_tests -j
./build/math-assurance/mathematical_assurance_tests
```

See [`docs/GLOBAL_MATHEMATICAL_ASSURANCE.md`](docs/GLOBAL_MATHEMATICAL_ASSURANCE.md).

## 2026-07-26 Scientific Fidelity and Predictive Accuracy Platform

The `aesim_advanced` library now exports an additive scientific-fidelity layer:

```cpp
#include "aesim/advanced/scientific_fidelity_platform.hpp"
```

It implements monolithic strongly coupled multiphysics, modal hp-adaptive DG
transport, complementarity contact, correlated spatial random fields and
uncertain geometry, ensemble field assimilation, PDE-constrained inversion,
Peng-Robinson real-fluid flash calculations, Bayesian multimodel averaging,
correlated total error budgets, virtual laboratory instrumentation, progressive
material damage, and mixed-mode cohesive fracture. Existing simulator features
and public APIs remain available.

Focused validation:

```bash
cmake -S . -B build/scientific-fidelity -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON \
  -DAESIM_BUILD_TOOLS=OFF -DAESIM_MAX_PARALLEL_COMPILES=2
cmake --build build/scientific-fidelity --parallel 2 --target \
  scientific_fidelity_platform_tests
ctest --test-dir build/scientific-fidelity --output-on-failure \
  -R '^scientific_fidelity_platform_(unit_tests|source_regression)$'
```

See [`docs/SCIENTIFIC_FIDELITY_PLATFORM.md`](docs/SCIENTIFIC_FIDELITY_PLATFORM.md)
and [`SCIENTIFIC_FIDELITY_PLATFORM_IMPLEMENTATION_REPORT_2026-07-26.md`](SCIENTIFIC_FIDELITY_PLATFORM_IMPLEMENTATION_REPORT_2026-07-26.md).

## 2026-07-26 Formula One multiphysics, optimization, and real-time platform

The `aesim_formula_one` library now exports a complete additive multiphysics layer:

```cpp
#include "aesim/advanced/formula_one_multiphysics_platform.hpp"
```

It implements `F1FlexibleBodyVehicleDynamics`,
`F1PersistentMultiCarWakeField`, `F1IntegratedThermalFluidNetwork`,
`F1PhysicsOfFailureLifing`, `F1OptimalExperimentDesigner`,
`F1AdvancedBayesianEstimator`, `F1AdaptiveMultifidelityManager`,
`F1DifferentiableFormulaOneRuntime`,
`F1CompressiblePowerUnitGasDynamics`, and
`F1RealtimeEcuHilIntegration`. These models add modal structural deformation,
persistent wake transport, pressure/enthalpy networks, mechanistic fatigue and
crack growth, information-optimal test selection, UKF and particle filtering,
validation-aware fidelity dispatch, exact second-order forward automatic
differentiation, finite-volume intake/exhaust dynamics, and deterministic ECU,
CAN, latency, deadline, and fault-injection behavior.

Focused validation:

```bash
cmake -S . -B build/f1-multiphysics -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON \
  -DAESIM_BUILD_TOOLS=OFF \
  -DAESIM_MAX_PARALLEL_COMPILES=2
cmake --build build/f1-multiphysics --parallel 2 --target \
  formula_one_multiphysics_platform_tests
ctest --test-dir build/f1-multiphysics --output-on-failure \
  -R '^formula_one_multiphysics_(platform_unit_tests|source_regression)$'
```

See **[`docs/FORMULA_ONE_MULTIPHYSICS_PLATFORM.md`](docs/FORMULA_ONE_MULTIPHYSICS_PLATFORM.md)**,
**[`FORMULA_ONE_MULTIPHYSICS_IMPLEMENTATION_REPORT_2026-07-26.md`](FORMULA_ONE_MULTIPHYSICS_IMPLEMENTATION_REPORT_2026-07-26.md)**,
and **[`FORMULA_ONE_MULTIPHYSICS_VALIDATION_2026-07-26.txt`](FORMULA_ONE_MULTIPHYSICS_VALIDATION_2026-07-26.txt)**.

## 2026-07-25 Formula One predictive-fidelity platform

The `aesim_formula_one` library now includes a complete, additive predictive-fidelity layer exported by:

```cpp
#include "aesim/advanced/formula_one_fidelity_platform.hpp"
```

The layer implements `F1FullyCoupledCarDynamicsKernel`,
`F1AdvancedTransientTyreModel`, `F1SensorDaqPipeline`,
`F1ClockSynchronizationEstimator`, `F1TelemetryStateParameterEstimator`,
`F1ValidationFramework`, `F1UncertaintyQuantificationFramework`, and
`F1IdentifiabilityFramework`. The implementation couples four transient tyre
models to six-degree-of-freedom body motion, suspension, wheel rotation,
aerodynamics, fuel use, and energy auditing. It also models sensor bias, drift,
noise, quantization, filtering, saturation, dropout, transport latency, clock
offset, and clock drift; performs nonlinear state and parameter estimation;
and supplies deterministic validation, Latin-hypercube uncertainty propagation,
and Fisher-information identifiability analysis.

No existing Formula One or simulator features were removed. The new source is
compiled into the existing `aesim_formula_one` target and exported transitively
through `aesim_advanced`.

Focused validation:

```bash
cmake -S . -B build/f1-fidelity -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON \
  -DAESIM_BUILD_TOOLS=OFF \
  -DAESIM_MAX_PARALLEL_COMPILES=2
cmake --build build/f1-fidelity --parallel 2 --target \
  formula_one_fidelity_platform_tests
ctest --test-dir build/f1-fidelity --output-on-failure \
  -R '^formula_one_fidelity_(platform_unit_tests|source_regression)$'
```

See **[`docs/FORMULA_ONE_FIDELITY_PLATFORM.md`](docs/FORMULA_ONE_FIDELITY_PLATFORM.md)**,
**[`FORMULA_ONE_FIDELITY_IMPLEMENTATION_REPORT_2026-07-25.md`](FORMULA_ONE_FIDELITY_IMPLEMENTATION_REPORT_2026-07-25.md)**,
and **[`FORMULA_ONE_FIDELITY_VALIDATION_2026-07-25.txt`](FORMULA_ONE_FIDELITY_VALIDATION_2026-07-25.txt)**.

## 2026-07-25 Formula One industrial correctness refactor

The Formula One industrial ecosystem now uses a deterministic global
maximum-cardinality, maximum-score driver-to-seat assignment engine. The prior
greedy allocator could consume the only rookie-qualified candidate on a
flexible seat and leave an FP1 rookie seat unfilled even though a complete
assignment existed. Medical fitness, budget, rookie, and Super-Licence rules
remain hard constraints, and output assignments remain in request seat order.

Tyre and sustainable-fuel release limits are validated once before processing,
including nonnegative metrology limits and ordered minimum/maximum windows.
Causal regression, linear-system elimination, aerodynamic aggregation,
efficiency, and scoring paths now reject non-finite intermediate results instead
of allowing overflow or NaN values to reach evidence generation.

Focused validation:

```bash
cmake -S . -B build/f1-industrial -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON \
  -DAESIM_BUILD_TOOLS=OFF \
  -DAESIM_MAX_PARALLEL_COMPILES=4
cmake --build build/f1-industrial --parallel 8 --target \
  formula_one_industrial_ecosystem_platform_tests
ctest --test-dir build/f1-industrial --output-on-failure \
  -R '^formula_one_industrial_ecosystem_(platform_unit_tests|source_regression)$'
```

See **[`DEBUG_REFACTOR_REPORT_2026-07-25.md`](DEBUG_REFACTOR_REPORT_2026-07-25.md)**
and **[`DEBUG_REFACTOR_VALIDATION_2026-07-25.txt`](DEBUG_REFACTOR_VALIDATION_2026-07-25.txt)**.

## 2026-07-24 debug and refactor hardening

The Formula One industrial ecosystem implementation now enforces finite
numerical outputs, identity uniqueness, uncertainty-valid metrology,
capacity-aware factory scheduling, compliance-first aerodynamic selection,
canonical missing-medical-response reporting, and strict driver medical and
FP1-rookie eligibility. The causal setup baseline no longer receives artificial
self-comparison uncertainty.

Ninja builds now default to a four-process C++ compile pool through
`AESIM_MAX_PARALLEL_COMPILES`. This prevents unrestricted `--parallel` builds
from exhausting memory on the project's feature-dense translation units while
leaving link and custom-command parallelism available. Use `0` to opt out.

Focused validation:

```bash
cmake -S . -B build/f1-industrial -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON \
  -DAESIM_MAX_PARALLEL_COMPILES=4
cmake --build build/f1-industrial --parallel 16 --target \
  formula_one_industrial_ecosystem_platform_tests
ctest --test-dir build/f1-industrial --output-on-failure \
  -R '^formula_one_industrial_ecosystem_platform_unit_tests$'
python3 tests/formula_one_industrial_ecosystem_source_regression.py .
```

See **[`DEBUG_REFACTOR_REPORT_2026-07-24.md`](DEBUG_REFACTOR_REPORT_2026-07-24.md)**
and **[`DEBUG_REFACTOR_VALIDATION_2026-07-24.txt`](DEBUG_REFACTOR_VALIDATION_2026-07-24.txt)**.


## 2026-07-27 IndyCar integrated fidelity platform

The sixth IndyCar module is exported through
`include/aesim/advanced/indycar_integrated_fidelity_platform.hpp` and compiled
into the existing `aesim_indycar` library. It implements a deterministic
multi-rate co-simulation runtime, telemetry Kalman assimilation and weighted
ridge calibration, a 22-degree-of-freedom multibody car, thermo-viscoelastic
combined-slip tires, unsteady modal aeroelastic aerodynamics, closed-loop ECU
and hybrid control, radio-semantic comprehension with probabilistic timing
fusion, multi-car pit-lane discrete-event scheduling, occupant/HANS/restraint
biomechanics, and deterministic uncertainty propagation with model-validity
supervision. Existing IndyCar modules and public APIs remain unchanged.

The advanced CLI exposes:

```bash
muzixdiagsys_advanced_platform indycar-integrated capabilities [output.json]
muzixdiagsys_advanced_platform indycar-integrated self-test DIRECTORY [output.json]
muzixdiagsys_advanced_platform indycar-integrated DOMAIN REQUEST.json OUTPUT.json [WORKING_DIRECTORY]
```

The ten domains are `integrated-cosimulation`, `telemetry-assimilation`,
`full-multibody`, `tire-contact`, `aeroelastic-aerodynamics`,
`ecu-hybrid-control`, `radio-timing`, `pit-lane-twin`,
`occupant-biomechanics`, and `uncertainty-validity`.

Focused validation:

```bash
cmake -S . -B build/indycar-integrated -G Ninja \
  -DCMAKE_BUILD_TYPE=Release -DBUILD_TESTING=ON \
  -DAESIM_ENABLE_SYCL=OFF -DAESIM_ENABLE_HIP=OFF
cmake --build build/indycar-integrated --parallel --target \
  aesim_indycar indycar_integrated_fidelity_platform_tests \
  muzixdiagsys_advanced_platform
ctest --test-dir build/indycar-integrated --output-on-failure \
  -R '^indycar_.*(unit_tests|source_regression)$'
```

See [`docs/INDYCAR_INTEGRATED_FIDELITY_PLATFORM.md`](docs/INDYCAR_INTEGRATED_FIDELITY_PLATFORM.md)
and [`examples/indycar_integrated_fidelity/`](examples/indycar_integrated_fidelity/)
for contracts, equations, canonical inputs, evidence behavior, and qualification
boundaries.

## 2026-07-28 IndyCar engineering assurance platform

The additive `indycar-assurance` command provides fourteen engineering-assurance domains without changing the existing IndyCar command families: effective-dated regulation resolution, dynamic legality drift, 2028 requirement/evidence certification, prospective manufacturer entry, probabilistic timing/video/telemetry fusion, officiating policy comparison, progressive contact damage and raceability, explicit crash/SAFER dynamics, coupled fire/rescue hazards, debris recovery, composite manufacturing, fleet reliability, D-optimal test design, and tire material genealogy/circularity.

The public API is `aesim/advanced/indycar_engineering_assurance_platform.hpp`; canonical requests are under `examples/indycar_engineering_assurance/`.

```bash
muzixdiagsys_advanced_platform indycar-assurance capabilities [output.json]
muzixdiagsys_advanced_platform indycar-assurance self-test DIRECTORY [output.json]
muzixdiagsys_advanced_platform indycar-assurance DOMAIN REQUEST.json OUTPUT.json [WORKING_DIRECTORY]
```

Focused validation target: `indycar_engineering_assurance_platform_tests`; source-completeness target: `indycar_engineering_assurance_source_regression`.

See [`docs/INDYCAR_ENGINEERING_ASSURANCE_PLATFORM.md`](docs/INDYCAR_ENGINEERING_ASSURANCE_PLATFORM.md), [`examples/indycar_engineering_assurance/`](examples/indycar_engineering_assurance/), and Chapter 60 of the user manual.

## 2026-07-23 IndyCar development and operations platform

The fifth IndyCar module is exported through `include/aesim/advanced/indycar_development_operations_platform.hpp` and compiled exclusively into `aesim_indycar`. It adds `IndyCarDevelopmentLadderPlatform`, `IndyCarFirestoneProductionMetrologyPlatform`, `IndyCarPowerUnitSupplyHomologationPlatform`, `IndyCarRenewableFuelLubricantLaboratory`, `IndyCarElectricalCyberPhysicalTwin`, `IndyCarRaceEngineeringIntelligence`, `IndyCarDriverSimulatorQualificationLaboratory`, `IndyCarTeamFactoryLogisticsTwin`, `IndyCarCircuitHomologationSafetyPlatform`, and `IndyCarMedicalOperationsBiomechanicsPlatform`.

The advanced CLI exposes:

```bash
muzixdiagsys_advanced_platform indycar-development capabilities [output.json]
muzixdiagsys_advanced_platform indycar-development self-test DIRECTORY [output.json]
muzixdiagsys_advanced_platform indycar-development DOMAIN REQUEST.json OUTPUT.json [WORKING_DIRECTORY]
```

The ten domains are `development-ladder`, `firestone-production`, `power-unit-supply`, `renewable-fuel-quality`, `electrical-cyberphysical`, `race-engineering-intelligence`, `driver-simulator-qualification`, `team-factory-logistics`, `circuit-homologation`, and `medical-operations`.

Focused validation:

```bash
cmake -S . -B build/indycar-development -G Ninja -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build/indycar-development --parallel --target aesim_indycar indycar_development_operations_platform_tests
ctest --test-dir build/indycar-development --output-on-failure -R '^indycar_.*_unit_tests$'
python3 tests/indycar_development_operations_source_regression.py .
```

See [`docs/INDYCAR_DEVELOPMENT_OPERATIONS_PLATFORM.md`](docs/INDYCAR_DEVELOPMENT_OPERATIONS_PLATFORM.md) for request contracts, algorithms, evidence behavior, exact commands, and qualification limits.


## 2026-07-27 NASCAR integrated-fidelity expansion


## 2026-07-28 NASCAR engineering assurance platform

The additive `nascar-assurance` command provides twelve new domains without changing the existing `nascar` or `nascar-integrated` contracts: effective-dated regulation resolution, dynamic post-race compliance, prospective OEM program management, probabilistic timing/SMT/video fusion, officiating policy comparison, progressive contact damage and raceability, explicit crash/SAFER elements, coupled fire/rescue hazards, debris recovery, composite manufacturing, fleet reliability, and D-optimal test design. The public API is `aesim/advanced/nascar_engineering_assurance_platform.hpp`; complete examples are under `examples/nascar_engineering_assurance/`. See [`docs/NASCAR_ENGINEERING_ASSURANCE_PLATFORM.md`](docs/NASCAR_ENGINEERING_ASSURANCE_PLATFORM.md) and Chapter 59 of the user manual.

Focused validation target: `nascar_engineering_assurance_platform_tests`; source completeness target: `nascar_engineering_assurance_source_regression`.

The additive `nascar-integrated` command provides twelve high-fidelity domains: deterministic multi-rate co-simulation, telemetry assimilation/calibration, correlated uncertainty and model-validity supervision, a flexible 28-DOF Next Gen vehicle, detailed asymmetric tire construction/contact, unsteady aeroelastic wakes and safety flaps, closed-loop ECU/sequential-transaxle/driveline control, cranktrain/dry-sump/fuel/thermal systems, a multi-car pit-road discrete-event twin, occupant biomechanics/heat strain/egress, scanned pavement mechanics, and multi-car spray/optical visibility. Existing `nascar` domains remain unchanged.

See [`docs/NASCAR_INTEGRATED_FIDELITY_PLATFORM.md`](docs/NASCAR_INTEGRATED_FIDELITY_PLATFORM.md) and Chapter 58 of the user manual for complete APIs, request contracts, equations, canonical examples, build/test commands, and qualification limits.

Focused validation target: `nascar_integrated_fidelity_platform_tests`; source completeness target: `nascar_integrated_fidelity_source_regression`.

## 2026-07-23 NASCAR next-generation engineering and operations expansion

The `aesim_nascar` library now includes a fourth additive platform exported by:

```cpp
#include "aesim/advanced/nascar_next_generation_platform.hpp"
```

The aggregate `nascar` command family now exposes 40 domains. The ten new domains are `electrified-stock-car`, `v8-combustion-fuel`, `aero-raceability`, `full-field-racecraft`, `remote-race-control`, `temporary-venue`, `wheel-end-durability`, `electrical-cyberphysical`, `race-engineering-intelligence`, and `broadcast-streaming`.

The implementation includes battery/motor/inverter electrothermal limits, cylinder-resolved sustainable-fuel V8 combustion, multi-car aerodynamic raceability, deterministic full-field racing, multimodal remote officiating, temporary-venue critical-path and evacuation analysis, brake/steering/single-lug durability, vehicle E/E and cyber fault propagation, uncertainty-qualified causal setup optimization, and end-to-end broadcast/CDN quality engineering. Each model performs bounded input validation and writes canonical SHA-256 evidence.

```bash
cmake -S . -B build/nascar -G Ninja -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build/nascar --parallel --target \
  aesim_nascar \
  nascar_next_generation_platform_tests
ctest --test-dir build/nascar --output-on-failure \
  -R '^nascar_next_generation_platform_unit_tests$'
python3 tests/nascar_next_generation_source_regression.py .
```

See [`docs/NASCAR_NEXT_GENERATION_PLATFORM.md`](docs/NASCAR_NEXT_GENERATION_PLATFORM.md) for complete request contracts, equations, outputs, qualification semantics, and validation commands.

## 2026-07-22 debug, refactor, and documentation refresh

The current source tree preserves the public simulator and advanced-platform command surfaces while correcting five substantive NASCAR frontier behaviors and one nondeterministic terminal-test harness. NASCAR sources are now isolated in the `aesim_nascar` static library, which is linked publicly by `aesim_advanced`; focused NASCAR tests no longer require the entire industrial and advanced dependency graph.

Key operator-visible semantics are now explicit:

- In-season championship probabilities are conditional on the surviving live bracket; eliminated drivers receive zero probability.
- Rule bulletins are validated before installation, and incompatible penalty ranges produce a failed adjudication with `recommended_penalty: null`.
- Fuel consumption records delivered fuel only; unavailable pickup demand is represented as starvation, not consumed mass.
- Failed logistics tasks consume neither parts nor resource capacity and cannot satisfy dependent tasks.
- `BUILD_TESTING` is the canonical CTest switch; the historical `AESIM_BUILD_TESTS` switch is mirrored for compatibility when supplied explicitly.

Focused validation:

```bash
cmake -S . -B build/nascar -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON \
  -DAESIM_ENABLE_SANITIZERS=ON \
  -DAESIM_ENABLE_HARDENING=OFF
cmake --build build/nascar --parallel --target \
  aesim_nascar \
  nascar_competition_platform_tests \
  nascar_ecosystem_platform_tests \
  nascar_frontier_platform_tests \
  nascar_next_generation_platform_tests
ctest --test-dir build/nascar --output-on-failure \
  -R '^nascar_.*_unit_tests$'
```

The validated complete matrix contains 157 registered tests: 156 passed, one optional Python runtime test was skipped because `gymnasium` was not installed, and no unresolved failures remain. See **[`DEBUG_REFACTOR_REPORT_2026-07-22.md`](DEBUG_REFACTOR_REPORT_2026-07-22.md)** and **[`DEBUG_REFACTOR_VALIDATION_2026-07-22.txt`](DEBUG_REFACTOR_VALIDATION_2026-07-22.txt)**.

## 2026-07-18 materials, energy, and multiphysics platform

MuzixDiagSys now includes mesh-free SPH/MPM/DEM mechanics, integrated computational materials engineering, manufacturing-process physics with as-built state reconstruction, switching-level power electronics, battery manufacturing and impedance diagnostics, environmental corrosion and water ingress, compressed and cryogenic hydrogen storage, discrete adjoints and SIMP topology optimization, polynomial-chaos and rare-event computing, and conservative finite-volume reacting-flow combustion. The implementation is additive and exported through `include/aesim/advanced/materials_energy_multiphysics_platform.hpp` and `include/aesim/advanced/platform.hpp`.

```bash
cmake --build build --target materials_energy_multiphysics_platform_tests -j
ctest --test-dir build -R materials_energy_multiphysics_platform_unit_tests --output-on-failure
```

See **[`docs/MATERIALS_ENERGY_MULTIPHYSICS_PLATFORM.md`](docs/MATERIALS_ENERGY_MULTIPHYSICS_PLATFORM.md)** and **[`MATERIALS_ENERGY_MULTIPHYSICS_PLATFORM_IMPLEMENTATION_REPORT_2026-07-18.md`](MATERIALS_ENERGY_MULTIPHYSICS_PLATFORM_IMPLEMENTATION_REPORT_2026-07-18.md)** for APIs, numerical methods, qualification boundaries, and validation details.

## 2026-07-18 qualification science, advanced materials, and autonomous testing platform

MuzixDiagSys now includes enforceable simulation-quality contracts, standards-oriented vehicle-dynamics signal validation, an executable regulation compiler with semantic dependency impact, composite laminate progressive damage, nonlinear monolithic aeroelasticity, viscoelastic tire-compound physics, thermo-elastohydrodynamic tribology, conformal surrogate certification with adaptive fidelity, delayed-feedback causal telemetry replay, and constrained D-optimal physical-test planning. The implementation is additive and exported through `include/aesim/advanced/qualification_science_platform.hpp` and `include/aesim/advanced/platform.hpp`.

```bash
cmake --build build --target qualification_science_platform_tests -j
ctest --test-dir build -R qualification_science_platform_unit_tests --output-on-failure
```

See **[`docs/QUALIFICATION_SCIENCE_PLATFORM.md`](docs/QUALIFICATION_SCIENCE_PLATFORM.md)** and **[`QUALIFICATION_SCIENCE_PLATFORM_IMPLEMENTATION_REPORT_2026-07-18.md`](QUALIFICATION_SCIENCE_PLATFORM_IMPLEMENTATION_REPORT_2026-07-18.md)** for APIs, equations, qualification boundaries, and validation details.

## 2026-07-18 Formula One design, test, and qualification platform

MuzixDiagSys now includes robust mixed-variable full-car multidisciplinary optimization, dynamic physical rig and deterministic HIL execution, uncertainty-aware digital scrutineering, virtual tire testing with nonlinear inverse identification, and Formula One control-software qualification with MIL/SIL equivalence, temporal requirements, fault campaigns, and safe-state analysis.

```bash
cmake --build build --target formula_one_design_qualification_tests -j
ctest --test-dir build -R formula_one_design_qualification_unit_tests --output-on-failure
```

See **[`docs/FORMULA_ONE_DESIGN_QUALIFICATION.md`](docs/FORMULA_ONE_DESIGN_QUALIFICATION.md)** for algorithms, APIs, workflows, evidence semantics, and qualification boundaries.

## 2026-07-18 Formula One team and competition digital twin

MuzixDiagSys now includes multi-car race dynamics and racecraft, dependency-driven pit-stop and garage operations, a versioned sporting/race-control/stewarding engine, uncertainty-qualified trackside metrology and correlation campaigns, and Bayesian competitor/game-theory/championship optimization. The built-in sporting profile identifies FIA 2026 Section B Issue 07; regulation logic is data-driven so later issues can be loaded without replacing the engine.

```bash
cmake --build build --target formula_one_team_competition_tests -j
ctest --test-dir build -R formula_one_team_competition_unit_tests --output-on-failure
```

See **[`docs/FORMULA_ONE_TEAM_COMPETITION.md`](docs/FORMULA_ONE_TEAM_COMPETITION.md)** for APIs, equations, workflows, evidence outputs, and scope boundaries.

## 2026-08-06 accuracy and performance hardening

The shared numerical and research runtimes have been further hardened without removing any command, model, UI surface, or simulation feature. Dense inversion now reuses one qualified factorization with per-column iterative refinement; complex residual certification uses overflow-resistant extended norms; pivoted QR uses scale-relative rank thresholds and QR-derived covariance; bounded Jacobians validate dimensions and finite stencils; Brent bracketing, adaptive quadrature, and Dormand-Prince integration handle floating-point edge cases more defensively; and the multi-rate scheduler performs checked deadline arithmetic with fewer redundant scans.

Research2 now routes dense solves through the qualified core, uses QR for GNSS and sim-to-real regression, applies Joseph-form EKF covariance updates, accumulates particle statistics without per-particle covariance temporaries, and evaluates Bayesian Mahalanobis/log-determinant terms from one scaled Cholesky factorization. The CLI remains a permanent first-class interface; beginner menus remain additive front ends to the same command dispatcher.

## 2026-07-18 global numerical rigor and mathematical qualification

MuzixDiagSys now applies a strict floating-point policy to every configured C++ target and provides a shared qualification-grade numerical kernel. The kernel includes compensated accumulation, stable online moments and covariance, equilibrated scaled-pivot dense real and complex solves with iterative refinement and condition diagnostics, column-pivoted Householder QR, bounded five-point Jacobians, Brent root finding, adaptive Gauss-Kronrod quadrature, adaptive Dormand-Prince integration, and invariant auditing.

The new mathematics has been integrated across calibration, uncertainty, measured validation, electrical networks, Modelica, sparse multiphysics, finite elements, electromagnetics, tires, reliability, surrogate analytics, Gaussian-process optimization, and Formula One correlation workflows. Existing APIs and model behavior remain available.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON \
  -DAESIM_ENABLE_STRICT_NUMERICS=ON
cmake --build build --target numerical_rigor_tests -j
ctest --test-dir build -R global_numerical_rigor_unit_tests --output-on-failure
```

See **[`docs/GLOBAL_NUMERICAL_RIGOR.md`](docs/GLOBAL_NUMERICAL_RIGOR.md)** for the algorithms, diagnostics, migration coverage, qualification workflow, and scope boundaries.

## 2026-07-17 deep engineering platform

MuzixDiagSys now includes a unified CSR sparse runtime with CG, GMRES, BiCGStab, Jacobi/ILU(0), Newton line search, implicit BDF2 integration, and adaptive tetrahedral refinement; rational NURBS and explicit B-rep topology with validation, healing, STEP polyhedral exchange, surface tessellation, and closed-shell volume meshing; transient unstructured CFD, conjugate heat transfer, and partitioned FSI; a full-system virtual ECU 3.0 with instruction-accurate RV32IM, hypervisor budgets, real-time scheduling, secure boot, cache/memory telemetry, peripherals, fault injection, and electrothermal behavior; and a solver-credibility laboratory with GCI, uncertainty propagation, Sobol indices, Bayesian calibration, and ensemble Kalman assimilation.

The public C++ API is declared in `include/aesim/advanced/deep_engineering_platform.hpp` and is re-exported by `include/aesim/advanced/platform.hpp`.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build --target deep_engineering_platform_tests -j
ctest --test-dir build -R deep_engineering_platform_unit_tests --output-on-failure
```

See **[`docs/DEEP_ENGINEERING_PLATFORM.md`](docs/DEEP_ENGINEERING_PLATFORM.md)** and **[`DEEP_ENGINEERING_PLATFORM_IMPLEMENTATION_REPORT_2026-07-17.md`](DEEP_ENGINEERING_PLATFORM_IMPLEMENTATION_REPORT_2026-07-17.md)** for algorithms, supported exchange profiles, numerical methods, qualification outputs, and validation details. Existing functionality remains available.

## 2026-07-16 must-have high-fidelity platform

MuzixDiagSys now includes a three-dimensional full-wave FDTD electromagnetic solver, a thin-wire antenna method-of-moments solver, EMC cable coupling, native multithreaded CPU execution, optional CUDA Driver API execution with concurrent multi-GPU partitioning, analytic CSG solids, tetrahedral volume meshing, unstructured thermal and structural finite elements, a multicore RV32IM virtual ECU with MMU/cache/ELF/DMA/CAN-FD/Ethernet behavior, flexible-ring tire and deformable-terrain physics, hydroplaning and adverse-weather behavior, and neural interval, branch-and-bound, adversarial, conformal, and closed-loop safety verification.

The public C++ API is declared in `include/aesim/advanced/must_have_platform.hpp` and is also included by `include/aesim/advanced/platform.hpp`.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build --target must_have_platform_tests -j
ctest --test-dir build -R must_have_platform_unit_tests --output-on-failure
```

See **[`docs/MUST_HAVE_PLATFORM.md`](docs/MUST_HAVE_PLATFORM.md)** and **[`MUST_HAVE_PLATFORM_IMPLEMENTATION_REPORT_2026-07-16.md`](MUST_HAVE_PLATFORM_IMPLEMENTATION_REPORT_2026-07-16.md)** for algorithms, API behavior, runtime GPU discovery, numerical scope, and validation details. Existing simulation and engineering functionality remains available.

## 2026-07-16 integrated frontier platform

MuzixDiagSys now includes a shared physically based spectral scene renderer for optical camera, thermal camera, multi-return lidar, and FMCW radar I/Q; a heterogeneous automotive SoC with coherent instruction-accurate RV32IM cores and functional DSP/GPU/NPU jobs; spatial porous-electrode battery chemistry and dynamic PEM fuel-cell physics; three-phase radial feeder power flow with deadline-aware charging and V2G; and a deterministic factory/supply-chain discrete-event twin.

The public C++ API is declared in `include/aesim/advanced/integrated_frontier_platform.hpp`. The implementation is documented in **[`docs/INTEGRATED_FRONTIER_PLATFORM.md`](docs/INTEGRATED_FRONTIER_PLATFORM.md)** and **[`INTEGRATED_FRONTIER_PLATFORM_IMPLEMENTATION_REPORT_2026-07-16.md`](INTEGRATED_FRONTIER_PLATFORM_IMPLEMENTATION_REPORT_2026-07-16.md)**. The registered validation target is `integrated_frontier_platform_unit_tests`. Existing simulation, engineering, diagnostics, qualification, plugin, FMI, SSP, AUTOSAR, and command functionality remains available.

## 2026-07-15 standards, deployment, and credibility platform

MuzixDiagSys now includes a deterministic OpenSCENARIO DSL compiler and elaborator, an OpenODD/ISO 34503-oriented operational-domain engine, an FMI 3.0 Scheduled Execution master, complete SSP 2.x topology/parameter/mapping/dictionary/resource round trips, a unified OpenX ontology, terminal and self-contained HTML ODD coverage studios, outward-rounded interval numerics, an in-process Boolean SMT and nonlinear delta-SAT backend, finite-state probabilistic model checking, certified linear model reduction, WCET/schedulability analysis, symbolic security-protocol verification, differentiable camera/radar/lidar rendering, EKF SLAM, RF/V2X/GNSS propagation, governed sim-to-real adaptation, game-theoretic traffic agents, and split/adaptive conformal calibration.

```text
muzixdiagsys_standards_deployment capabilities
muzixdiagsys_standards_deployment self-test
muzixdiagsys_standards_deployment compile-scenario scenario.osc scenario.json
muzixdiagsys_standards_deployment compile-scenario scenario.osc scenario.xosc
```

The public C++ API is declared in `include/aesim/research2/standards_deployment_platform.hpp`. See **[`docs/STANDARDS_DEPLOYMENT_CREDIBILITY_PLATFORM.md`](docs/STANDARDS_DEPLOYMENT_CREDIBILITY_PLATFORM.md)** for the supported language and package profiles, algorithms, numerical guarantees, examples, deterministic behavior, validation coverage, and explicit engineering scope boundaries.

## 2026-07-15 advanced safety discovery and remediation platform

MuzixDiagSys now includes integrated search-guided falsification, counterfactual intervention planning, dynamic cross-domain fault propagation, distribution-aware regression gating, an interactive reverse debugger, explicit model validity governance, predictive runtime safety shields, formal hybrid reachability, resilient controller synthesis, saltation-aware hybrid differentiation, executable safety cases, risk-weighted requirement coverage, deterministic distributed execution, deterministic heterogeneous/GPU auditing, online digital-twin state and parameter assimilation, Gaussian-process model discrepancy, adaptive multi-fidelity execution, and a unified SQLite experiment database.

```text
muzixdiagsys_advanced_safety capabilities
muzixdiagsys_advanced_safety self-test
muzixdiagsys_advanced_safety debugger [timeline.json]
```

The new C++ API is declared in `include/aesim/research2/advanced_safety_platform.hpp`. See **[`docs/ADVANCED_SAFETY_DISCOVERY_PLATFORM.md`](docs/ADVANCED_SAFETY_DISCOVERY_PLATFORM.md)** for algorithms, APIs, deterministic guarantees, command usage, persistence behavior, and validation coverage.

## 2026-07-14 high-frequency simulation performance refactor

The flexible-ring tire, conservative multi-rate scheduler, integrated road-profile coupling, and uncertain-sensor acquisition paths have been refactored to remove repeated allocation, sorting, interpolation, trigonometry, associative lookup, and output copying from high-frequency execution. Existing commands, aliases, owning input APIs, and model behavior remain available.

On deterministic GCC 14.2 `-O3` microbenchmarks, the tire step improved by **9.63×**, scheduler dispatch by **1.61×**, and four-channel sensor acquisition by **1.33×**, with identical benchmark checksums. Allocation instrumentation reduced 1,000 warmed tire-step allocations from 1,000 to zero and scheduler allocations from 39,999 to zero. The complete CTest suite passes **111/111**.

See **[`reports/PERFORMANCE_DEBUG_REFACTOR_2026-07-14.md`](reports/PERFORMANCE_DEBUG_REFACTOR_2026-07-14.md)** for the implementation analysis, benchmark methodology, compatibility details, and limitations, and **[`FINAL_PERFORMANCE_VALIDATION_2026-07-14.txt`](FINAL_PERFORMANCE_VALIDATION_2026-07-14.txt)** for the concise validation record.

## 2026-07-14 canonical command discovery and contextual Tab inspector

The interactive command system now presents one authoritative spelling for each behavior while preserving every established command path. The root registry contains 164 canonical commands and 49 compatibility aliases. Compatibility aliases remain executable for scripts, journals, saved workflows, and operator muscle memory, but they are omitted from Tab completion, the command palette, schema path enumeration, and generated discovery lists. Pressing Tab on an exact legacy alias migrates the editor to its canonical spelling. Engine and vehicle preset nicknames follow the same migration policy.

Tab completion now opens a responsive split inspector:

- The left pane contains canonical candidates only and follows the active pointer.
- The right pane shows the selected command's category, concise purpose, operational details, compatibility aliases, valid next tokens, insertion behavior, and discovery policy.
- Tab, Shift-Tab, Up, Down, Home, and End move the pointer and refresh the description immediately.
- PageUp/PageDown scroll the selected command description independently.
- The mouse wheel moves the candidate pointer when it is over the left pane and scrolls the description when it is over the right pane.
- Narrow terminals automatically stack the candidate and description regions instead of truncating the inspector.
- Misspelled root commands receive bounded fuzzy recovery against canonical commands only.
- Command dispatch now normalizes aliases once at admission and routes only canonical roots internally, eliminating duplicated alias conditionals from domain handlers.
- Settable scalar parameters are intentionally discoverable beneath `set <Tab>` rather than polluting the root command list.

Use `command-schema status`, `command-schema validate`, and `command-schema aliases` to inspect the canonical registry, validate metadata/grammar coverage, and view every accepted compatibility migration. No executable feature or compatibility spelling was removed. See **[`docs/COMMAND_REGISTRY_AND_COMPLETION.md`](docs/COMMAND_REGISTRY_AND_COMPLETION.md)** and **[`reports/COMMAND_UI_CONTEXTUAL_COMPLETION_2026-07-14.md`](reports/COMMAND_UI_CONTEXTUAL_COMPLETION_2026-07-14.md)**.


## 2026-07-18 Formula One performance, correlation, and driver laboratory

The advanced Formula One platform now includes a sequential gearbox/final-drive/differential/clutch and launch laboratory, wind-tunnel/CFD/track aerodynamic correlation, driver behavior and biomechanics with driver-in-the-loop session analysis, cooling/package/mass/ballast co-optimization, and cylinder-resolved sustainable-fuel combustion with turbo gas-path dynamics. All systems are additive and provide validated configuration guards, structured documents, and deterministic evidence hashes.

See **[`docs/FORMULA_ONE_PERFORMANCE_LABORATORY.md`](docs/FORMULA_ONE_PERFORMANCE_LABORATORY.md)** and build `formula_one_performance_laboratory_tests` for the dedicated regression suite.

## 2026-07-14 reliability and filesystem-safety maintenance

This maintenance pass preserves the existing simulator, engineering, diagnostics, authentication, plugin, FMI, Python, terminal, and test command surfaces while hardening two shared infrastructure paths:

- Atomic document replacement now creates staging files exclusively, writes through an already-open native file handle, flushes data before replacement, removes abandoned staging files through RAII cleanup, preserves process-default permissions for ordinary new outputs, preserves an existing destination's POSIX permission bits, and provides an owner-private path for security-sensitive files.
- Authentication initialization now restricts only directories created by MuzixDiagSys. A custom database path inside an existing shared or administrator-managed directory no longer causes the application to replace that parent directory's permissions. The user database itself remains owner-private.
- Regression coverage verifies concurrent atomic writers, staging-file cleanup, owner-private security writes, destination-permission preservation, empty-path rejection, non-destructive custom authentication paths, and private permissions for newly created authentication directories.

See **[`reports/DEBUG_REFACTOR_FILESYSTEM_SAFETY_2026-07-14.md`](reports/DEBUG_REFACTOR_FILESYSTEM_SAFETY_2026-07-14.md)** for the defect analysis and implementation details, and **[`FINAL_VALIDATION_2026-07-14.txt`](FINAL_VALIDATION_2026-07-14.txt)** for the exact build, regression, sanitizer, and environment record.

## 2026-07-14 validation lifecycle and digital engineering

The authenticated engineering platform now includes formal temporal requirements and runtime monitors, Latin-hypercube/Sobol uncertainty analysis, automatic global-plus-local calibration, persisted quadratic surrogates and multi-fidelity arbitration, maximin/D-optimal experiment design, hash-sealed safety cases, coupled EV thermal/HVAC networks, battery degradation and safety state, event-driven ECU/CAN timing, deterministic SIL/PIL/HIL execution with loopback or UDP I/O, correlated virtual fleets, stabilized predictive maintenance and RUL, FFT/order-based NVH analysis, physical bounds and conservation checks, immutable collaborative reviews, and a persistent engineering knowledge graph.

```text
muzixdiagsys_engineering --credential-file credentials.txt requirements evaluate requirements.json trace.json result.json
muzixdiagsys_engineering --credential-file credentials.txt uncertainty run study.json uncertainty.json
muzixdiagsys_engineering --credential-file credentials.txt timing run timing.json timing-result.json
muzixdiagsys_engineering --credential-file credentials.txt xil execute xil.json xil-result.json
muzixdiagsys_engineering --credential-file credentials.txt collaboration verify reviews REQ-001
```

See **[`docs/VALIDATION_LIFECYCLE_PLATFORM.md`](docs/VALIDATION_LIFECYCLE_PLATFORM.md)** for schemas, algorithms, RBAC behavior, C++ and Python APIs, XIL transport configuration, and validation procedures.

## 2026-07-14 integrated engineering platform

The authenticated release now includes a production `aesim_engineering` library, the `muzixdiagsys_engineering` command surface, and the `muzixdiag` Python package. These integrate role-based permissions, cross-process tamper-evident audit logs, workspace membership and sealed reproducibility manifests, unit-aware scenario composition, local/distributed campaign execution, heterogeneous compute backends, deterministic replay, composable fault injection, hash-sealed TCP telemetry, diagnostic test planning, recursive run comparison and multi-format reports, FMI/OpenSCENARIO/OpenDRIVE adapters, interactive courses, typed calculations, deterministic driver profiles, and a multi-rate sensor suite. Existing simulator, project, checkpoint, OpenX, FMI, diagnostics, plugin, API, and terminal functionality remains available.

```text
muzixdiagsys_engineering --credential-file credentials.txt roles catalog
muzixdiagsys_engineering --credential-file credentials.txt workspace list workspaces
muzixdiagsys_engineering --credential-file credentials.txt campaign execute campaign.json result.json
muzixdiagsys_engineering --credential-file credentials.txt audit verify
```

See **[`docs/ENGINEERING_PLATFORM.md`](docs/ENGINEERING_PLATFORM.md)** for security behavior, data formats, distributed workers, Python usage, and complete command examples.

## 2026-07-14 authenticated operator access

MuzixDiagSys now requires operator authentication before starting the simulation thread, dashboard, batch command processor, API server, or diagnostic command dispatcher. The bootstrap account is `jtmuzix`; its initial password is `T1k1@420`, and it has user-management permission. Passwords are stored only as salted PBKDF2-HMAC-SHA-256 verifiers with 600,000 iterations. New accounts **cannot** create users unless an authorized administrator explicitly delegates that right.

```text
user whoami
user list
user create technician1
user create supervisor1 --can-create-users
user permission technician1 on
user disable technician1
user passwd
logout
```

Interactive passwords are entered without terminal echo. Protected automation can use `--auth-user` with `--auth-password-file`, or `--auth-credential-file`. See [`docs/AUTHENTICATION.md`](docs/AUTHENTICATION.md) for database locations, security controls, command syntax, and automation guidance. Change the bootstrap password after first deployment.

## 2026-07-13 first-class projects and diagnostic workbench

MuzixDiagSys now provides a versioned, portable `.muzixproj` workspace format (`muzixdiagsys.project` 1.0.0), nine resumable guided diagnostic workflows, and a typed causal-diagnostics graph. Existing checkpoint, scenario, plugin, fault, OBD, UDS, DoIP, SOVD, logging, and terminal commands remain available.

A project persists vehicle and engine selection, parameter overrides, active plugins, ECU/network topology, injected faults, scenario and random seed, imported datasets with SHA-256 integrity, named watch lists, terminal layout, named and active-state checkpoints, generated artifacts, and the complete active workflow case. Paths are made project-relative when possible, saves are atomic, and loads are transactional with rollback on failed validation or restoration.

```text
project new cases/no_start.muzixproj No_Start_Case
project set seed 4242
project dataset add data/measured_validation_example.csv measured-validation
project watch create diagnostics
project watch select diagnostics
project watch add engine_rpm
project checkpoint add known-good Before fault injection
workflow start crank-no-start CASE-NS-001
workflow requests
workflow evaluate
causal report crank-no-start
workflow report reports/CASE-NS-001.md
causal json reports/CASE-NS-001-graph.json crank-no-start
project save
project validate cases/no_start.muzixproj
```

Implemented workflow IDs are `crank-no-start`, `lean-operation`, `rich-operation`, `misfire`, `low-fuel-pressure`, `boost-control-deviation`, `catalyst-efficiency`, `ev-isolation`, and `can-communication`. Every workflow includes preconditions, diagnostic requests, quantitative expectations, pass/fail branching, evidence capture, candidate causes, confirming tests, repair verification, resumable JSON state, and Markdown report generation.

The causal graph represents symptoms, DTCs, freeze frames, sensors, actuators, wiring/network paths, operating conditions, candidate root causes, and confirming tests. Nodes and conclusions are explicitly classified as `fact`, `model-derived`, `heuristic`, or `missing`; ranked causes retain supporting, contradicting, and required-test relationships instead of being mislabeled as facts.

See [`docs/PROJECT_DIAGNOSTIC_WORKBENCH.md`](docs/PROJECT_DIAGNOSTIC_WORKBENCH.md), [`schemas/muzixproj.schema.json`](schemas/muzixproj.schema.json), and [`reports/MUZIXDIAGSYS_PROJECT_WORKFLOW_CAUSAL_IMPLEMENTATION_2026-07-13.md`](reports/MUZIXDIAGSYS_PROJECT_WORKFLOW_CAUSAL_IMPLEMENTATION_2026-07-13.md).

## 2026-07-13 deterministic network fault laboratory

The live automotive network stack now includes a stateful `NetworkFaultLaboratory` shared by CAN/CAN-FD, ISO-TP/UDS, DoIP, SOME/IP-SD, Ethernet, and TSN paths. It provides controllable congestion, error-passive and bus-off transitions, frame loss/delay/duplication/reordering, rolling-counter and checksum corruption, gateway routing errors, CAN-FD incompatibility, ISO-TP sequence and Flow Control failures, DoIP activation rejection, SOME/IP service instability, Ethernet jitter, and TSN deadline/gate violations. Existing behavior is unchanged when no network fault is enabled.

```text
networklab reset 4242
networklab set can-bus-off 1 1 tx node=gateway recovery_ms=500
networklab can-probe tx 0x7E0 02 01 0C
networklab node gateway
networklab recover gateway
networklab set isotp-flow-control 1 1 tx action=overflow
networklab isotp-probe tx 22 F1 90 4D 55 5A 49 58 44 49 41 47 53 59 53
networklab events 20
project fault add network.frame-drop 0.8 probability=0.05 scope=rx
project save
```

`netfault` is an exact alias. Laboratory state is serialized into `.muzixproj` metadata together with deterministic RNG position, pending delayed/reordered traffic, CAN controller counters, evidence events, and statistics. The guided `can-communication` workflow consumes measured drop ratios, routing/protocol failures, controller state, and TSN violations.

See [`docs/NETWORK_FAULT_LABORATORY.md`](docs/NETWORK_FAULT_LABORATORY.md), [`examples/reference_network_fault_lab.json`](examples/reference_network_fault_lab.json), and [`reports/MUZIXDIAGSYS_NETWORK_FAULT_LAB_IMPLEMENTATION_2026-07-13.md`](reports/MUZIXDIAGSYS_NETWORK_FAULT_LAB_IMPLEMENTATION_2026-07-13.md).

## 2026-07-13 diagnostic architecture, reliability, and documentation revision

This release consolidates diagnostic semantics in `aesim::industrial::DiagnosticService`. CLI requests, the guarded CAN/OBD gateway, vehicle-side responder, ELM327-compatible adapter, DoIP facade, SOVD facade, and diagnostic tests now share ECU identity, PID, VIN, DTC, MIL, readiness, freeze-frame, UDS, and clear behavior. The compatibility facade in `include/modules/can_uds.hpp` is implemented in `src/industrial/diagnostic_compat.cpp` rather than maintaining an independent header-only protocol stack.

Mode 02 freeze-frame lifecycle is corrected: a clean-to-confirmed-fault transition captures the pre-fault snapshot, active confirmed faults preserve it, clearing the confirmed list resets it, and the next independent episode captures new data. Mixed-case filesystem paths are preserved for affected export commands. Build-footprint, package-membership, manual, command-completion, and mixed-case-path regressions protect these changes.

Operator entry points:

```text
diagnostics topology
diagnostics obd powertrain 010C
diagnostics uds powertrain 22F190
elm ATZ
elm 010C
doip 10 22F190
sovd GET /entities
validation measured data/measured_validation_example.csv time_s measured_torque_nm simulated_torque_nm weight reports/measured_validation.json reports/measured_residuals.csv
```

Detailed operating and validation guidance is in the regenerated User Manual and the synchronized CAN/OBD, SocketCAN responder, and command-registry documents.

## 2026-07-10 Professional simulation-platform implementation

This release adds a complete professional execution and interoperability layer without removing the established simulator, research core, command families, file formats, ABI-v1 plugins, FMI workflow, or regression coverage. The new implementation is built as the `aesim_professional` C++17 library and is consumed by the existing `muzixdiagsys` executable.

### Full-state checkpoints, branches, and deterministic replay

Complete checkpoint images include plant and controller state, the modular research core, multi-rate scheduler state, random streams, DTC and freeze-frame memory, numerical-health rolling windows, MIL/SIL state, and serializable plugin state. Checkpoint integrity is protected by SHA-256 and schema validation.

```text
checkpoint status
checkpoint save run.aecp
checkpoint verify run.aecp
checkpoint inspect run.aecp
checkpoint load run.aecp
branch create baseline
branch create candidate
branch compare baseline candidate
branch load baseline
replay start run.aereplay
step 0.050
replay stop
replay verify run.aereplay
```

Replay files embed their initial full-state checkpoint and verify the deterministic state hash after every recorded command. Host wall-clock performance counters remain in checkpoints for diagnostics but are deliberately excluded from trajectory-equivalence hashes because they do not affect simulated physics.

### Strong physical dimensions and unit conversion

Subsystem interfaces use compile-time quantity types for pressure, temperature, torque, force, power, energy, mass, mass flow, time, angular speed, distance, velocity, area, and dimensionless values. The unit registry performs checked SI conversion at file, command, controller, plugin, and scenario boundaries and rejects incompatible dimensions.

### Versioned schemas and migrations

```text
schema2 list
schema2 validate scenario.yaml aesim.scenario
schema2 migrate old_config.json config_v2.json aesim.config
schema2 migrate old_calibration.json calibration_v2.json aesim.calibration
schema2 dump aesim.checkpoint
```

Current schemas are `aesim.config` 2.0.0, `aesim.calibration` 2.0.0, `aesim.scenario` 2.0.0, and `aesim.checkpoint` 3.0.0. Major-version migration is explicit and validated after every transformation.

### Continuous conservation and numerical health

The health monitor evaluates mass, energy, and torque closure together with local integration error, rejected steps, nonlinear iterations, map extrapolations, state clamps, and deadline misses. It retains rolling histories in full-state checkpoints and can mark a run warning, invalid, or abort-requested according to configurable limits.

```text
health status
health json reports/health.json
health limits 0.005 0.020 0.010 0.050 5 20
health reset
```

### Declarative scenarios and temporal assertions

Versioned YAML or JSON scenarios support timed and condition-triggered events, unit-aware set operations, ramps, commands, checkpoint and branch events, stop conditions, and `always`, `eventually`, and `at_end` assertions with warning, error, or abort severity.

```text
scenario2 validate experiments/transient.yaml
scenario2 run experiments/transient.yaml reports/scenario_result.json
```

### Plugin ABI v2 and process isolation

ABI v1 remains supported. ABI v2 adds structure-size/version negotiation, capability discovery, explicit execution phases, deterministic state serialization, typed step contexts, timeout/error accounting, and both in-process and supervised out-of-process execution. Process mode uses bounded IPC, heartbeat/timeout handling, crash containment, and checkpointable plugin state.

```text
plugin v2 abi
plugin v2 load build/plugins/libaesim_sample_native_plugin_v2.so process {} 4242
plugin v2 status
plugin v2 timeout 100
plugin v2 unload
```

### FMI 3 model import and export

The simulator exports a binary FMI 3 package with Model Exchange, Co-Simulation, and Scheduled Execution interfaces, continuous-state derivatives and ModelStructure metadata, resources, documentation, and portable serialized FMU state. The importer supports stored and Deflate-compressed FMUs, validates CRCs and extraction limits, blocks path traversal, loads the current-host binary, and operationally executes all three interface types.

```text
fmi3 export aesim_powertrain.fmu
fmi3 inspect aesim_powertrain.fmu
fmi3 import aesim_powertrain.fmu cs
fmi3 step 0.010 55 20
fmi3 unload
fmi3 import aesim_powertrain.fmu me
fmi3 import aesim_powertrain.fmu se
fmi3 cosim aesim_powertrain.fmu 2.0 0.001 fmi3_trace.csv
```

The build requires zlib for bounded ZIP/Deflate handling. Exported binary FMUs contain the current host-platform binary; build/package the project on each target platform when a multi-platform FMU is required.

### MIL and SIL execution

The execution manager provides deterministic integer-time controller scheduling in `legacy`, `mil`, `sil`, `shadow_mil`, and `shadow_sil` modes. Typed controller inputs/outputs, period control, deadline statistics, serializable controller state, and a stable production-controller C ABI form the base for future PIL/HIL adapters. Shadow modes calculate and compare controller output without applying it to the plant.

```text
execution status
execution mode mil
execution period 0.001
execution mil configure controller.json
execution sil load build/controllers/libaesim_sample_sil_controller.so {} 12345
execution mode sil
execution mode shadow_sil
execution sil unload
```

The regression matrix includes `professional_core_unit_tests` and `professional_platform_v2_regression`, which validate exact state continuation, schema migration, health-history restoration, scenario temporal semantics, process-isolated plugins, MIL/SIL restoration, all three FMI interfaces, FMU state restoration, and Deflate-compressed FMU import.



## 2026-07-09 Research-level implementation expansion

This build adds a fully executable research-level modeling and diagnostics layer on top of the previously optimized simulator. Existing command families, regression tests, README command coverage, professional logging, dataset export, stability auditing, scenario execution, and prior physics/control features are preserved.

Implemented additions:

- Validation, parameter identification, and uncertainty quantification: `identify fit friction <coastdown.csv>`, `identify fit dyno [trace.csv] [iterations]`, `identify fit telemetry [iterations]`, `identify report [path.md]`, `uncertainty montecarlo <n> <out.csv>`, and `uncertainty sobol <n> <out.csv>` now execute deterministic runtime identification and uncertainty studies with simulator-state restoration after each trial.
- Multi-zone combustion, knock, and abnormal-combustion modeling: `combustion model two_zone|multi_zone`, `combustion zones <n>`, `combustion residual <fraction>`, `combustion egr <fraction>`, and `combustion knock_model none|integral|surrogate` extend the crank-angle combustion trace with burned/unburned zone temperatures, residual/EGR effects, end-gas autoignition index, pre-ignition probability, misfire probability, IMEP, COV of IMEP, and per-cylinder imbalance metrics.
- High-fidelity thermal-fluid network with component aging: `thermal pump <pct>`, `thermal aging on|off`, `thermal service`, and `thermal fouling <radiator> <oil_cooler> <intercooler>` add coolant/oil flow, piston temperature, heat-exchanger fouling, coolant degradation, oil-viscosity response, head/piston/turbo/catalyst damage accumulation, and service reset behavior to the existing thermal-network command family.
- Advanced emissions and aftertreatment: `emissions model simple|thermal|aftertreatment|research`, `emissions aging <0..1>`, `emissions oxygen <0..1>`, `emissions capacity <g>`, `emissions cycle <out.csv>`, `emissions export <out.csv>`, and `emissions report` now expose catalyst oxygen storage, aging authority, cold/thermal conversion behavior, and cumulative HC/CO/NOx/CO2 reporting.
- Crankshaft torsion, NVH, firing-order, and cylinder imbalance: `nvh model simple|torsional`, `nvh firing_order <sequence>`, `nvh segments <n>`, `nvh stiffness <Nm_per_rad>`, `nvh damping <Nms_per_rad>`, `nvh imbalance <pct>`, and `nvh export <out.csv>` now compute firing frequency, crank twist, speed ripple, order amplitudes, roughness, misfire signature, and cylinder imbalance effects.
- Advanced drivetrain and vehicle dynamics: `tire dynamics longitudinal|bicycle`, `tire wheelbase <m>`, `tire cg_height <m>`, `tire brake_bias <front_fraction>`, `tire model simple|pacejka_lite|brush`, `tire export <out.csv>`, and `chassis export <out.csv>` now include bicycle-model lateral response, slip angle, yaw rate, lateral acceleration, load-transfer-related state, brake bias, and expanded tire/chassis telemetry.
- CAN/OBD/J1939 diagnostic simulation and fault injection: `fault inject <fault_name> <severity>`, `fault clear all`, `dtc inject <code> <description>`, `obd mode 01|02|03|04|06`, `j1939 status`, and `j1939 export <out.csv>` now provide state-affecting faults, DTC/freeze-frame behavior, OBD service responses, and J1939-style PGN/SPN diagnostic snapshots. Supported runtime fault effects include boost leak, MAF/MAP/lambda/coolant bias, thermostat stuck open, catalyst efficiency loss, CAN dropout, injector imbalance, misfire, brake fade, and tire-mu degradation.
- Research-grade solver framework: `solver rk45`, `solver tolerance abs|rel <value>`, `solver mindt <seconds>`, `solver events on|off`, and `solver status` extend the solver with adaptive-step control, error tracking, minimum-step limits, rejected-step counting, and event-detection accounting while preserving Euler, semi-implicit, RK2, and RK4 modes.

Representative research command sequence:

```text
quickstart
combustion model multi_zone
combustion zones 5
combustion residual 0.08
combustion egr 0.12
combustion knock_model integral
combustion export combustion_research.csv
thermal model network
thermal pump 72
thermal aging on
thermal fouling 0.05 0.02 0.03
thermal export thermal_research.csv
emissions model aftertreatment
emissions cycle emissions_cycle.csv
nvh model torsional
nvh firing_order 1-3-4-2
nvh segments 5
nvh imbalance 10
nvh export nvh_research.csv
tire model brush
tire dynamics bicycle
tire wheelbase 2.70
tire export tire_research.csv
chassis export chassis_research.csv
fault inject boost_leak 0.35
dtc active
obd mode 03
j1939 export j1939_research.csv
solver rk45
solver tolerance abs 0.00001
solver events on
solver status
uncertainty montecarlo 4 uq.csv
identify fit friction coastdown.csv
identify report identify.md
```

The regression suite includes `research_level_regression`, which exercises the new command families and validates that exported CSV/Markdown artifacts contain research-specific columns such as `end_gas_autoignition_index`, `preignition_probability`, `imep_bar`, `piston_c`, `coolant_flow_kg_s`, `head_damage`, `nox_g_s`, `cumulative_co2_g`, `crank_twist_deg`, `speed_ripple_rpm`, `cylinder_imbalance_pct`, `vehicle_model`, `slip_angle_deg`, `yaw_rate_deg_s`, `pgn`, `spn`, `trial`, `method`, `peak_torque_nm`, and `knock_max`.

## 2026-07-09 Professional optimization and invariant-audit expansion

This build adds concrete simulator improvements focused on repeatability, observability, and numerical robustness. No existing features were removed.

Implemented additions:

- Enhanced professional logger: `log remove <channel...>`, `log set <channel...>`, `log stats`, and `log export markdown <path.md>` now provide channel curation, duplicate-safe channel selection, descriptive statistics, and human-readable signal-log export in addition to the existing CSV/JSONL outputs.
- Expanded live signal registry: `dataset stats` and `dataset export json|markdown <path>` now expose a richer one-shot signal surface covering ECU torque demand/limits, turbo speed and pressure ratio, air-path state, combustion metrics, thermal network nodes, tire/chassis state, emissions, NVH, wear, and core engine channels.
- Numerical/physical invariant auditing: `stability audit`, `stability check`, `stability report`, and `stability export <csv>` evaluate runtime bounds and consistency checks for power conversion, RPM, torque, lambda, MAP/MAF, temperatures, oil pressure, fuel tank state, gear validity, tire friction/slip, turbo speed/PR, combustion pressure/knock, catalyst temperature, and thermal-network nodes.
- Deterministic design-of-experiments sweeps: `sweep throttle <start_pct> <end_pct> <points> <hold_s> <out.csv>` and `sweep spark <start_deg> <end_deg> <points> <hold_s> <out.csv>` perform fully executable runtime sweeps and export measured engine, ECU, turbo, combustion, thermal, chassis, and tire responses.
- Combustion trace allocation optimization: the crank-angle combustion trace now reserves the required vector capacity before regeneration, reducing repeated allocation overhead in high-rate research/fidelity modes while preserving the existing trace output.

Representative command sequence:

```text
quickstart
log set rpm torque_nm speed boost lambda thermal_head turbo_rpm compressor_pr
log start 200
throttle 65
step 0.35
log stop
log stats
log export markdown opt_log.md
dataset stats
dataset export json dataset_snapshot.json
stability audit
stability export stability.csv
sweep throttle 10 70 4 0.05 throttle_sweep.csv
sweep spark 6 18 4 0.05 spark_sweep.csv
```

The regression suite includes `professional_optimization_regression`, which validates the new logger statistics/export paths, dataset JSON export, invariant-audit CSV output, and both throttle and spark sweeps.

## 2026-07-09 Professional feature implementation expansion

This build adds the requested professional physics/control command families as executable simulator features, not placeholders. Existing command surfaces remain available.

Implemented additions:

- Advanced combustion model: `combustion model simple|map|wiebe|advanced`, `combustion spark <deg_btdc>`, `combustion burn <deg_ca>`, `combustion step <deg_ca>`, and `combustion export <trace.csv>` for crank-angle pressure/heat-release traces.
- Real torque-based ECU architecture: `ecu torque_model on|off`, `ecu pedal_map linear|sport|eco`, `ecu torque_request <Nm>`, `ecu lambda_target <lambda>`, `ecu boost_target <kPa>`, `ecu limiter list|enable limp|disable limp`, and `ecu spark_strategy mbt|knock_limited|fixed`. The ECU computes driver demand, wheel/engine torque request, air-charge request, actuator targets, and active torque limiters.
- Turbocharger and intake/exhaust gas path: `turbo status`, `turbo load compressor|turbine <csv>`, `turbo boost_target <kPa>`, `turbo intercooler <eff>`, `turbo vvt <intake> <exhaust>`, `turbo egr <pct>`, and `turbo export <csv>`. The report and export include shaft speed, compressor/turbine efficiency, pressure ratio, surge/choke margin, wastegate/bypass, exhaust pressure, outlet temperature, MAP, MAF, and VE.
- Drivetrain, tire, and chassis expansion: `tire model simple|pacejka_lite|brush`, `tire mu <value>`, `tire abs on|off`, `tire esc on|off`, `tire diff open|lsd|locked`, `tire export <csv>`, plus `chassis mass|cda|grade|rr|brake|export`. The vehicle update loop now uses the tire force envelope, ABS brake limiting, brake heating/fade, aero downforce, load transfer, traction intervention, and chassis grade/road-load state.
- Thermal network controls: `thermal status`, `thermal model simple|network`, `thermal fan auto|on|off|<pct>`, `thermal radiator <eff>`, `thermal oil_cooler <eff>`, `thermal intercooler <eff>`, and `thermal export <csv>`. The runtime thermal loop applies control efficiencies to coolant/oil/exhaust coupling.
- Professional CLI families: `log`, `dataset`, `benchmark`, `profile`, `calibrate`, and `explain` are now executable. `log` records selected signal channels and exports CSV/JSONL; `dataset export` writes a current signal snapshot; `benchmark run` advances the model and records runtime metrics; `profile run` reports benchmark plus subsystem state; `calibrate` wraps fitting/optimization; `explain` provides subsystem provenance/status views.

Representative command sequence:

```text
quickstart
throttle 80
ecu torque_model on
ecu pedal_map sport
ecu torque_request 420
step 0.2
combustion model advanced
combustion export combustion_trace.csv
turbo boost_target 150
turbo export turbo_snapshot.csv
thermal model network
thermal fan on
thermal export thermal_snapshot.csv
tire model pacejka_lite
tire mu 0.62
abs off
chassis grade 4
step 0.3
tire export tire_snapshot.csv
log start 50
step 0.3
log export csv signal_log.csv
dataset export dataset_snapshot.csv
benchmark run 0.05 benchmark.csv
profile run 0.05
explain ecu
```

The regression suite includes `professional_feature_regression`, which verifies the command family behavior and confirms that the documented CSV/JSONL artifacts are actually written.

## 2026-07-09 Professional operations expansion

This build adds another fully executable professional-operations layer without removing existing simulator behavior:

- Model documentation generator: `docs generate <dir>`, `docs dictionary <path.md>`, `docs commands <path.md>`, `docs schemas <path.md>`, and `docs model <path.md>`.
- Configuration migration tool: `config migrate <input> <output> [kind]`, `config check-version <file>`, `config diff <old> <new>`, and `config upgrade-all <dir> [out_dir]`.
- Safety envelope monitor: `safety status`, `safety limits`, `safety watch on|off`, `safety set <metric> <field> <value>`, `safety export <csv>`, and `safety import <csv>`.
- Professional doctor command: `doctor` and `doctor verbose` check resources, schemas, plugin ABI, writable paths, dictionary availability, real-time scheduling, and safety-limit initialization.
- Failure-injection campaign generator: `fault campaign generate <file.yaml>`, `fault campaign run <file.yaml> <out_dir>`, and `fault campaign report`.

Example:

```text
doctor
docs generate docs_generated
config migrate data/scenario_example.yaml migrated_scenario.yaml scenario
safety status
safety export safety_limits.csv
fault campaign generate fault_campaign.yaml
fault campaign run fault_campaign.yaml campaign_out
```

The regression suite includes `professional_ops_regression`, which exercises all five new operational subsystems end-to-end and verifies generated artifacts.

## 2026-07-09 Real-world calibration/debug update

This build was rechecked against public 2024 Volkswagen Golf GTI technical-specification anchors and the regression suite was expanded.  Updates include:

- Recalibrated the default 2.0 L turbo GTI-style full-load torque curve toward the public 241 hp / 273 lb-ft production anchors.
- Corrected the EA888-style default geometry/compression anchor to 9.6:1.
- Updated default boost authority to the public 32.9 psi maximum-turbo-boost anchor, represented internally as approximately 226.8 kPa gauge.
- Updated Volkswagen Golf GTI Mk8 vehicle presets:
  - DSG curb mass: 1446 kg.
  - Manual curb mass: 1423 kg.
  - 7-speed DSG ratios: 3.40 / 2.75 / 1.76 / 0.92 / 0.70 / 0.75 / 0.63.
  - 6-speed manual ratios: 3.77 / 2.09 / 1.48 / 1.09 / 1.10 / 0.91.
  - Reverse ratios and Final I / Final II values updated from the public VW technical sheet.
- Added optional per-gear final-drive support for dual-final transmissions.
- Updated GTI CdA estimates using VW drag-coefficient values and the public Golf frontal-area reference.
- Relaxed the coastdown regression to verify progressive downshifting as speed/RPM decay rather than forcing an unrealistic immediate 6->5 shift at the first sample.
- Added `realworld_gti_spec_regression`, which validates the GTI preset anchors and the full-load dyno-reference CSV.

Run the full validation suite with:

```bash
cmake -S . -B build
cmake --build build -j
ctest --test-dir build --output-on-failure
```


Research-oriented C++17 terminal simulator for engine, ECM, fuel, transmission, vehicle, diagnostics, visualization, and repeatable experiment workflows.

## Build

Debug/development build:

```bash
cmake -S . -B build/debug -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
CTEST_PARALLEL_LEVEL="$(nproc)" \
  cmake --build build/debug --target aesim_check --parallel "$(nproc)"
./build/debug/muzixdiagsys
```

Optimized portable build:

```bash
cmake -S . -B build/release -DCMAKE_BUILD_TYPE=Release -DBUILD_TESTING=ON
CTEST_PARALLEL_LEVEL="$(nproc)" \
  cmake --build build/release --target aesim_check --parallel "$(nproc)"
```

The `aesim_check` target is transactional: all libraries, tools, plugins, and test executables are built before CTest starts. This prevents one compiler error from being obscured by a cascade of `Could not find executable` failures. The equivalent convenience wrapper is `tools/build_full_and_test.sh --clean`. Direct `ctest` invocations are also protected by the `aesim_prepare_test_artifacts` setup fixture, which incrementally builds the same artifact closure before selected tests run; see `docs/CTEST_ARTIFACT_FIXTURE.md`.

Optional build controls are `AESIM_ENABLE_HARDENING` (default `ON`),
`AESIM_ENABLE_POSITION_INDEPENDENT_CODE` (default `ON`),
`AESIM_ENABLE_SANITIZERS`, `AESIM_ENABLE_LTO`, and
`AESIM_ENABLE_NATIVE_OPTIMIZATION`. Position-independent code is enabled for
all static libraries and executables so Clang/GCC builds remain compatible with
PIE-by-default distributions and the `lld` linker. Native CPU optimization is
disabled by default so packaged binaries remain portable. Sanitizer builds
should normally disable hardening to simplify diagnostics:

```bash
cmake -S . -B build/sanitize -DCMAKE_BUILD_TYPE=Debug \
  -DBUILD_TESTING=ON -DAESIM_ENABLE_SANITIZERS=ON \
  -DAESIM_ENABLE_HARDENING=OFF
CTEST_PARALLEL_LEVEL="$(nproc)" \
  cmake --build build/sanitize --target aesim_check --parallel "$(nproc)"
```


### Complete Formula One, IndyCar, and NASCAR build/test sequence

Formula One sources are compiled directly into `aesim_advanced`. All six IndyCar modules are compiled into the focused `aesim_indycar` library, and all five NASCAR modules are compiled into `aesim_nascar`; both focused libraries are linked transitively and publicly by `aesim_advanced`. The following portable sequence disables only optional SYCL/HIP discovery:

```bash
rm -rf build/motorsport
cmake -S . -B build/motorsport -G Ninja \
  -DCMAKE_BUILD_TYPE=RelWithDebInfo \
  -DBUILD_TESTING=ON \
  -DAESIM_BUILD_TOOLS=ON \
  -DAESIM_ENABLE_HARDENING=ON \
  -DAESIM_ENABLE_POSITION_INDEPENDENT_CODE=ON \
  -DAESIM_ENABLE_STRICT_NUMERICS=ON \
  -DAESIM_ENABLE_SYCL=OFF \
  -DAESIM_ENABLE_HIP=OFF
cmake --build build/motorsport --parallel "$(nproc)"

cmake --build build/motorsport --parallel "$(nproc)" --target \
  formula_one_platform_tests \
  formula_one_race_engineering_tests \
  formula_one_performance_laboratory_tests \
  formula_one_team_competition_tests \
  formula_one_design_qualification_tests \
  formula_one_frontier_laboratory_tests \
  formula_one_physical_operations_laboratory_tests \
  indycar_platform_tests \
  indycar_operations_platform_tests \
  indycar_future_competition_platform_tests \
  indycar_frontier_expansion_platform_tests \
  nascar_competition_platform_tests \
  nascar_ecosystem_platform_tests \
  nascar_frontier_platform_tests

ctest --test-dir build/motorsport --output-on-failure \
  -R '^formula_one_.*_unit_tests$'
ctest --test-dir build/motorsport --output-on-failure \
  -R '^indycar_.*_unit_tests$'
ctest --test-dir build/motorsport --output-on-failure \
  -R '^nascar_.*_unit_tests$'
ctest --test-dir build/motorsport --output-on-failure
./build/motorsport/muzixdiagsys
```

See Chapters 2 and 29-47 of the comprehensive user manual for prerequisites, sanitizer commands, platform descriptions, corrected NASCAR semantics, and individual validation targets.



## IndyCar Future Competition and Development Platform

The advanced library now includes a 2028 next-generation vehicle and transition laboratory; charter, Leaders Circle, championship, manufacturer, and entrant economics; official timing, photo finish, and stewarding; a layered Firestone structural tyre model; fuel-cell slosh and mass migration; trackside safety and restart readiness; an executable IRIS rule/bulletin compiler; suspension K&C and seven-post correlation; multi-car team strategy; and regulated wind-tunnel/straight-line aero development. See `docs/INDYCAR_FUTURE_COMPETITION_PLATFORM.md`.

## IndyCar Frontier Expansion Platform

The fourth IndyCar module is exported by:

```cpp
#include "aesim/advanced/indycar_frontier_expansion_platform.hpp"
```

It fully implements ten additional systems: a cylinder-resolved 2028 2.4-liter power-unit and homologation laboratory; twenty-cell ultracapacitor, MGU, and inverter electrothermal simulation; sequential gearbox, clutch, bellhousing, differential, and driveline durability; hydraulic and carbon-brake physics; laser-scanned grip/weather evolution; deterministic 2-35 car racecraft; synchronized camera/telemetry incident reconstruction; pit-lane computer-vision officiating; appeals and precedent auditing; and the complete Indianapolis 500 Month-of-May programme. See [`docs/INDYCAR_FRONTIER_EXPANSION_PLATFORM.md`](docs/INDYCAR_FRONTIER_EXPANSION_PLATFORM.md) and [`examples/indycar_frontier_expansion/`](examples/indycar_frontier_expansion/).

Build the focused IndyCar library and run the dedicated regression without compiling unrelated advanced-platform modules:

```bash
cmake --build build/motorsport --target \
  aesim_indycar \
  indycar_frontier_expansion_platform_tests --parallel "$(nproc)"
ctest --test-dir build/motorsport --output-on-failure \
  -R '^indycar_frontier_expansion_platform_unit_tests$'
```

### Clang/lld position-independent build

A clean Clang + `lld` build is supported directly. Do not reuse an older build
directory because CMake does not retroactively recompile archive members after
position-independent-code policy changes.

```bash
rm -rf build/clang-lld
CC=clang CXX=clang++ cmake -G Ninja -S . -B build/clang-lld \
  -DCMAKE_BUILD_TYPE=RelWithDebInfo \
  -DBUILD_TESTING=ON \
  -DAESIM_ENABLE_POSITION_INDEPENDENT_CODE=ON \
  -DCMAKE_EXE_LINKER_FLAGS=-fuse-ld=lld \
  -DCMAKE_SHARED_LINKER_FLAGS=-fuse-ld=lld
cmake --build build/clang-lld --parallel
ctest --test-dir build/clang-lld --output-on-failure
```

If a downstream packaging environment intentionally requires a non-PIE
executable, it may set `-DAESIM_ENABLE_POSITION_INDEPENDENT_CODE=OFF` and must
also disable that environment's PIE link policy. The supported and hardened
default remains PIC/PIE enabled.

Startup help:

```bash
./build/muzixdiagsys --help
./build/muzixdiagsys -h
./build/muzixdiagsys --advanced-help
```

## Runtime behavior

The simulator starts safely:

- loop stopped
- monitor/dashboard idle
- key off
- no injected failures
- no active P-codes

Use `loop start` to run continuously or `step <seconds>` to advance manually. In an interactive POSIX terminal, the dashboard remains fixed at the top; the lower Command Activity pane supports mouse-wheel/PageUp/PageDown scrollback.

The dashboard renderer is intentionally non-flickering: after the first paint it no longer clears the entire terminal on every loop tick. It homes the cursor, overwrites the dashboard/output frame in place, clears only the current row tails, and performs a full clear only on first draw or terminal-size changes. This keeps `loop start` visually stable while metrics update in place.

## Major implemented systems

### 2026-07-09 Research physics and instrumentation expansion

This build adds fully executable research-oriented subsystems rather than empty command shells:

- Runtime provenance/equation tracing through `trace <term>` for torque, wheel force, boost, air path, combustion, thermal behavior, sensors, and CAN.
- Crank-angle-resolved combustion through `combustion status`, including Wiebe heat release, MFB10/MFB50/MFB90, pressure trace preview, peak pressure angle, pressure-rise rate, ringing index, and knock index.
- Transient turbocharger dynamics through `turbo status`, including shaft inertia, compressor/turbine power balance, compressor outlet temperature, boost-control error, PID-style wastegate motion, bypass behavior, surge/choke margin, and overspeed warnings.
- Dynamic air-path modeling through `airpath status`, `airpath vvt <intake> <exhaust>`, `airpath egr <pct>`, and `airpath intercooler <pct>`, coupling manifold filling, VE, VVT, EGR, intercooler efficiency, MAF, and exhaust-manifold pressure.
- Multi-node thermal network through `thermalnet`, tracking block, head, coolant, oil, exhaust manifold, turbo CHRA, catalyst, ATF, intercooler, radiator outlet, thermostat, fan, and rejected heat.
- Sensor and actuator realism through `sensor` and `actuator` commands, with noise, bias, lag, dropout, stuck-value faults, authority limits, and actuator rate limits.
- CAN timing/arbitration/fault simulation through `can bus`, including periodic frames, arbitration ordering, bus-load estimate, and frame drop/delay/corruption fault injection.

Representative command sequence:

```text
quickstart
throttle 55
step 1
trace torque
trace boost
trace combustion
combustion spark 16
airpath vvt 20 -8
airpath egr 8
thermalnet
sensor fault map bias 2
actuator fault throttle authority 0.8
can bus fault 0x0C0 corrupt 1
step 0.1
can bus
```

The regression suite includes `research_features_regression`, which exercises these command paths and verifies that the outputs are real subsystem reports.


### OBD-II live data mode

Commands:

```text
obd
obd live
obd live 2.0 5
obd pids
obd pid 010C
obd raw 010C
obd pid 0105
obd pid 010B
obd pid 0110
obd export data/obd_snapshot.csv
```

The OBD subsystem now returns decoded values and raw SAE Mode 01 style ECU frames. Supported values include monitor status/MIL count, calculated load, RPM, vehicle speed, coolant temperature, MAP, intake temperature, MAF, throttle position, runtime, fuel level proxy, module voltage, absolute load, commanded equivalence ratio, ambient temperature, oil temperature, and fuel rate. `obd live <seconds> <Hz>` captures a short live trace by advancing the simulator and printing decoded values plus raw response bytes.

### Multi-fidelity modes

```text
fidelity status
fidelity simple
fidelity standard
fidelity advanced
fidelity research
```

Fidelity now changes both numerical staging and model coupling. `simple` is a fast map-centric mode that suppresses wear-induced secondary faults for quick what-if work. `standard` runs the fuel-system, thermal, DTC, vehicle, TCS/ABS, and normal wear path. `advanced` tightens internal stage size and strengthens wear/failure coupling. `research` enforces the finest built-in substepping, full fuel/wear/thermal/scope coupling, and the most deterministic behavior for repeatable studies.

### Research numerical solver modes

```text
solver status
solver euler
solver semi_implicit
solver rk2
solver rk4
solver dt 0.005
solver substeps 4
```

The solver setting combines with fidelity mode to select substep behavior for real-time or research-style integration. The `solver dt` control bounds the maximum internal stage size, and `solver substeps` enforces a minimum stage count for reproducible high-resolution integration.

### ECU calibration profiles

```text
cal status
cal stock
cal economy
cal sport
cal track
cal valet
cal limp
```

Profiles alter throttle authority, boost authority, spark/lambda bias, and shift aggressiveness. They are not labels only; the selected profile changes the control path used by the simulation.

### Real ECM strategy modes

```text
ecm
ecm status
ecm modes
ecm directory
```

Implemented ECM modes include key-off, cranking, after-start, warmup open-loop, open-loop, closed-loop, idle control, decel fuel cut, power enrichment, knock-limited, rev-limit, limp-home, over-temperature, oil-pressure protection, low-fuel-pressure, no-crank-sync, and stall. Modes affect throttle authority, idle airflow, decel fuel cut, rev/protection torque limiting, and no-crank-sync behavior.

### Energy-balance report

```text
energy
energy export data/energy_ledger.csv
view energy
```

Reports a first-law energy ledger: fuel chemical power, indicated work, brake shaft work, motoring absorption, coolant/block heat, oil/lube heat, exhaust/other heat, FMEP friction loss, PMEP pumping loss, accessory load, combustion residual, closure error, brake thermal efficiency, indicated thermal efficiency, and mechanical efficiency. `energy export` writes the current ledger to CSV.

### Numerical stability audit

```text
audit
view audit
```

Checks physical and numerical plausibility: finite RPM/MAP/lambda, bounded temperatures, plausible fuel flow, plausible vehicle acceleration, tire friction, brake thermal efficiency, and first-law residual behavior.

### Data recorder / oscilloscope mode

```text
scope status
scope add rpm
scope add boost
scope add lambda
scope add fuel_pressure
scope rate 100
scope trigger rpm above 1200
scope start
step 2.0
scope stop
scope view
scope trend rpm
scope hist fuel_pressure
scope export data/scope.csv
scope clear
```

Default channels include RPM, torque, horsepower, boost, lambda, coolant, oil pressure, and vehicle speed. The recorder supports manual recording, trigger-armed recording, CSV export, recent-sample table view, sparkline trends, and channel histograms. Supported channel names include RPM, torque, HP, boost, MAP, lambda, AFR, MAF, coolant, oil, oil_pressure, EGT, speed, gear, throttle, fuel_flow, fuel_pressure, fuel_level, pump_duty, injector_pw, fuel_temp, battery, slip, accel, BTE, knock, misfire, TCC slip, and ATF temperature.

### Visual system pages

```text
view main
view engine
view fuel
view energy
view obd
view scope
view vehicle
view tire
view wear
view audit
view hist
view visual
view gauges
view expert
```

These complement the pinned dashboard and histogram views. `view visual`, `view gauges`, and `view expert` display a compact expert gauge wall with colorized bars for powertrain, air/fuel, thermal, energy-closure, and tire metrics.

### Realistic fuel system

```text
fuels
fuel premium_93
fuel properties
fuel system
fuel tank 10
fuel refuel 20
fuel capacity 55
fuelprops
fuel custom octane=94 ethanol=15
```

Fuel properties affect stoichiometric AFR, LHV, density, octane/knock resistance, charge-cooling proxy, flame-speed proxy, high-load torque factor, BSFC, fuel flow, and lambda behavior. The fuel subsystem now includes tank volume, fuel consumption, low-fuel starvation, pump enable/duty, low-pressure rail dynamics, direct-injection high-pressure rail proxy, fuel temperature, vapor-lock margin, injector pulse width, injector deadtime, fuel per injection event, ethanol sensing, learned stoich AFR, and lambda-trim reporting. Low fuel or vapor-lock conditions alter rail pressure, lambda, misfire rate, torque, and DTC behavior.

### Engine wear and degradation

```text
wear status
wear run 10000
wear maintenance oil
wear maintenance plugs
wear maintenance injectors
wear maintenance coolant
wear maintenance turbo
wear maintenance all
wear reset
```

Wear accumulates with simulated time/distance and affects the physical model through ring wear, bearing wear, injector deposits, plug wear, turbo wear, cooling scale, catalyst aging, oil age, and derived failure severities. The wear report now includes retained compression, oil-pressure retention, injector-flow retention, ignition-energy retention, cooling-capacity retention, turbo-efficiency retention, and service flags. Severe aging can generate realistic condition-based DTCs through the same diagnostic path as injected failures.

### Monte Carlo simulation

```text
montecarlo 100
montecarlo 500
montecarlo export 1000 data/montecarlo.csv
```

Runs deterministic-seed uncertainty analysis over ambient pressure, ambient temperature, humidity, AKI octane, ethanol percentage, compressor efficiency, intercooler effectiveness, boost leak, injector restriction, compression scatter, and road friction. Reports mean, standard deviation, 5th/50th/95th percentiles, risk probabilities for knock-limited operation, high EGT, lean mixture, underboost, and misfire, plus histogram bars. `montecarlo export` writes per-run CSV data for external analysis.

### Vehicle and tire dynamics

```text
vehicle
road surface dry
road surface wet
road surface snow
road surface ice
traction on
traction off
abs on
abs off
```

Model includes effective tire friction, road wetness, front-drive traction limit, longitudinal weight-transfer proxy, wheel speed, slip ratio, traction-control intervention, ABS intervention, rolling resistance, aerodynamic drag, grade force, brake force, and acceleration.

## Existing retained features

The update preserves existing commands and workflows:

- pinned dashboard
- scrollable lower Command Activity pane
- arrow-key history
- tab completion
- engine presets including Volkswagen GTI 2.0 TSI EA888 evo4 aliases
- fuel-grade effects
- manual/automatic transmission
- key/start/shutdown workflow
- failure injection and repair
- DTC/P-code directory
- dyno sweep and dyno histogram
- validation against dyno CSV
- histogram output
- parameter tweaking via `set`

## Example workflows

### GTI calibration experiment

```text
engine gti
fuel premium_93
cal sport
fidelity research
solver rk4
quickstart
step 1.0
throttle 80
step 2.0
energy
audit
obd live
```

### Failure + OBD/DTC workflow

```text
engine gti
fuel regular_87
quickstart
step 1.0
throttle 70
fail boost_leak 0.55
step 1.0
diagnostics
dtc active
obd live
repair all
```

### Scope recorder workflow

```text
scope add rpm
scope add boost
scope add lambda
scope rate 50
scope start
quickstart
step 2.0
throttle 60
step 3.0
scope stop
scope view
scope export data/scope_run.csv
```

### Wear/degradation workflow

```text
wear status
wear run 50000
wear status
quickstart
step 1.0
diagnostics
wear maintenance all
wear status
```

## Accuracy note

This is a non-proprietary research surrogate. It uses physically grounded approximations, built-in calibration maps, and public-output anchors where available. Exact production accuracy for a specific vehicle still requires measured ECU maps, dyno data, combustion pressure traces, injector characterization, turbo compressor/turbine maps, emissions hardware data, and validation logs for that exact vehicle.

## Latest professional/research-grade implementation pass

This build adds five concrete systems without removing the prior simulator features.

### 1. Report generator

The simulator can now generate Markdown engineering reports directly from the current simulator state.

Commands:

```text
report help
report session reports/session.md
report energy reports/energy.md
report dyno reports/dyno.md
report validation reports/validation.md data/vw_gti_ea888_evo4_dyno.csv
report diagnostics reports/diagnostics.md
report preview session
```

Reports include configuration summary, solver/fidelity state, engine/fuel/vehicle data, OBD-II output, energy balance, calibration-map summary, diagnostics, wear state, and dyno/validation sections depending on report type.

### 2. Regression test suite

CTest is now integrated. The suite includes:

- C++ unit/quantity and calibration-map tests.
- CLI regression test covering startup DTC state, `--help`, OBD/energy/map/unit/report commands, calibration export, and Markdown report generation.

Run:

```bash
cmake -S . -B build
cmake --build build -j
ctest --test-dir build --output-on-failure
```

### 3. Unit / quantity safety system

A lightweight compile-time quantity system is included under `include/core/units.hpp`. It provides typed wrappers and conversions for pressure, temperature, torque, power, mass flow, energy, speed, volume, and distance.

Interactive command:

```text
units
view units
```

The simulator uses this for unit-auditable power and energy calculations, and the regression test suite compiles these types separately to catch unit-conversion regressions.

### 4. Full calibration-map framework

The simulator now supports inspection, sampling, loading, and exporting of rectangular 2D calibration maps.

Supported maps:

```text
bmep / torque
bsfc
ve
egt
mfb50
```

Commands:

```text
map list
map inspect bmep
map sample bmep 1600 1.0 clamp
map sample bmep 7200 1.1 extrapolate
map load bmep data/my_bmep_map.csv
map export bmep data/exported_bmep.csv
loadmap bmep data/my_bmep_map.csv
view maps
```

CSV format:

```csv
rpm_or_x,load_or_y,value
1000,0.0,-1.2
1000,0.2,2.0
...
```

The loader requires a complete rectangular grid and rejects duplicate or missing calibration cells. Runtime sampling supports bounded/clamped lookup and analysis-grade linear edge extrapolation.

### 5. Bottom-pane flicker fix

Interactive rendering now builds a complete row model but transmits only rows whose content changed. Dashboard ticks therefore avoid repainting unchanged command activity and editor rows. Initial display, terminal resize, modal overlays, screen-reader mode, or a frame with more than 45% changed rows safely triggers a complete redraw; all other frames use synchronized dirty-row patches and restore the editor cursor.


## 2026-07-09 Research-grade modular systems upgrade

This version adds five concrete systems without removing existing commands or workflows.

### 1. Modularized codebase

New subsystem headers live under `include/modules/`:

```text
include/modules/vehicle_presets.hpp
include/modules/emissions.hpp
include/modules/can_uds.hpp
include/modules/validation_suite.hpp
```

The main simulator still builds as a single executable, but vehicle configuration, catalyst/emissions math, CAN/UDS diagnostics, and validation reporting are now separated into reusable modules with independent regression coverage.

### 2. Full vehicle presets

Built-in vehicle presets now apply mass, tire radius, aerodynamic road load, rolling resistance, brake force, driveline loss, final drive, reverse gear, transmission efficiency, and gear-ratio sets.

Commands:

```text
vehicle
vehicle list
vehicle generic_sedan
vehicle vw_gti_mk8_manual
vehicle vw_gti_mk8_dsg
vehicle sport_coupe
vehicle pickup_tow
vehicle dyno_cell
```

Manual vehicles use clutch **pedal-depression** semantics:

```text
key start          # starter automatically holds the clutch at 100% depressed
clutch 0           # release the pedal / couple the driveline for acceleration
clutch 100         # depress before every gear change
shift up
clutch 0           # release again after the shift
```

The `clutch` command is rejected and omitted from Tab completion and the command palette while an automatic transmission is selected.

All 24 vehicle presets and all 19 engine presets are loaded from the single authoritative YAML catalog `configs/powertrain_catalog.yaml`. The runtime validates types, physical ranges, unique keys/aliases, transmission mode, complete gearing, and every vehicle-to-engine reference before exposing a preset.

### 3. Catalyst / emissions model

The catalyst model tracks catalyst temperature, light-off, conversion efficiency, upstream/downstream lambda, instantaneous CO2/CO/HC/NOx/PM rates, cumulative mass, and a P0420 catalyst-efficiency proxy. It uses fuel flow, lambda, EGT, coolant temperature, vehicle speed, fuel LHV, ethanol fraction, and compression-ignition bias.

Commands:

```text
emissions
emissions export data/emissions.csv
```

### 4. CAN / OBD-II / UDS diagnostics

The simulator now emits realistic encoded CAN OBD-II request/response frames and supports a compact UDS diagnostic layer.

Commands:

```text
obd
obd pids
obd pid 010C
can
uds services
uds session default
uds session extended
uds read_did F190
uds read_did F187
uds read_did F18C
uds read_did F40D
uds read_dtc
dtc active
```

Supported Mode 01 PIDs include RPM, speed, coolant temperature, MAP, MAF, throttle position, commanded lambda, fuel rate, catalyst temperature, ambient temperature, and control-module voltage.

### 5. Formal validation suite

The validation suite now checks multi-domain simulator sanity instead of only dyno curve agreement. It validates physical ranges for engine state, thermal state, vehicle parameters, catalyst state, emissions rates, OBD payload encoding, and transmission configuration.

Commands:

```text
validate suite
validate export reports/validation.md
validation
validation export reports/validation.md
```

CTest now covers the modular subsystems:

```bash
cmake -S . -B build
cmake --build build -j
ctest --test-dir build --output-on-failure
```

## Restored interactive dashboard, shell history, completion, and advanced help

This update restores the previously available terminal UI while keeping the newer modular vehicle, emissions, CAN/UDS, validation, report, unit, and calibration-map features.

Restored UI features:

```text
dashboard | dash | metrics      Refresh the fixed dashboard
loop start                      Run the simulation without scrolling telemetry spam
loop stop                       Stop the simulation loop
output clear                    Clear the lower Command Activity pane
scroll up|down|pageup|pagedown  Scroll only the lower Command Activity pane
scroll top|bottom               Jump lower-pane scrollback
```

Interactive POSIX terminal behavior:

- The dashboard is pinned at the top of the screen.
- Press `h` on an empty command line to hide it and expand the Command Activity pane; press `s` on an empty command line to restore it.
- A leading space keeps `h`- or `s`-prefixed commands in command-entry mode, and normal characters remain unchanged after command entry begins.
- The lower Command Activity pane scrolls independently and preserves its top-line anchor while the dashboard is toggled.
- The loop updates dashboard values in place instead of printing repeated output.
- Up/down arrows recall command history.
- Left/right arrows edit the active command line.
- Tab completion covers commands, subcommands, fuels, vehicles, OBD/UDS terms, maps, reports, and settable parameters.
- Mouse wheel and PageUp/PageDown scroll the lower pane without moving the dashboard.
- Command history is saved to `.muzixdiagsys_history`; `.engine_sim_history` is imported as a legacy migration fallback.

Advanced startup help is restored:

```bash
./build/muzixdiagsys --help
./build/muzixdiagsys -h
./build/muzixdiagsys --advanced-help
```

Inside the simulator:

```text
help
help advanced
help all
```

## Advanced research-grade systems added in this build

This build adds concrete, executable implementations for the requested advanced systems while preserving the restored dashboard, scrollback pane, command history, tab completion, advanced `--help`, vehicle presets, emissions, CAN/UDS, validation, report generation, unit safety, and calibration-map features.

### Full Transmission Control Module

The TCM is now a real controller with shift strategy, commanded gear, shift phase, line pressure, clutch pressure, TCC lockup, converter slip, ATF temperature, kickdown logic, torque-reduction requests, adaptive reset, and transmission DTC integration.

```text
tcm status
tcm mode eco
tcm mode normal
tcm mode sport
tcm mode manual
tcm adapt reset
tcm lockup auto
tcm lockup force_on
tcm lockup force_off
```

### Drive-cycle simulation

Built-in cycles are executable with closed-loop speed tracking. The cycle runner commands throttle/brake, advances the simulation, accumulates distance, fuel, CO2, speed-tracking error, shifts, and readiness state.

```text
cycle list
cycle run urban
cycle run wltp
cycle run hwyfet
cycle run us06
cycle run data/custom_cycle.csv
```

Custom cycle CSV format:

```csv
time_s,speed_kmh
0,0
10,35
40,70
80,0
```

The loader accepts the documented `time_s,speed_kmh` header (or a legacy
headerless two-column trace), blank lines, and `#` comment lines. Malformed
rows, repeated headers after data begins, and unexpected third-column data are
rejected with the exact source line number instead of being skipped silently.

### Freeze-frame DTC records

DTCs now capture freeze-frame data at first trigger, including time, RPM, throttle, speed, gear, MAP, boost, lambda, coolant temperature, oil pressure, and trigger context.

```text
dtc active
dtc freeze
dtc freeze P0302
dtc clear all
```

### Turbo compressor and turbine map ingestion

The turbo subsystem now includes compressor/turbine efficiency, pressure ratio, corrected flow, shaft speed, wastegate position, surge margin, choke margin, exhaust manifold pressure, and DTC integration for abnormal loaded operation.

```text
turbo status
turbo load compressor data/sample_compressor_map.csv
turbo load turbine data/sample_turbine_map.csv
```

Turbo map CSV format:

```csv
flow_g_s,pressure_ratio,speed_krpm,efficiency
60,1.6,95,0.70
110,2.0,135,0.75
```

### Per-cylinder diagnostic testing

The simulator now tracks cylinder-specific compression, injector health, ignition health, contribution, IMEP, peak pressure, lambda, EGT, misfire probability, leakdown, and fault labels.

```text
cyl status
cyl balance
cyl compression_test
cyl leakdown_test
cyl 2 fail coil 0.60
cyl 3 fail injector 0.40
cyl repair all
```

Cylinder misfire thresholds generate cylinder-specific P030x records with freeze-frame capture.

### Coastdown and road-load estimation

The coastdown model simulates drag and rolling-resistance deceleration from a chosen starting speed and reports estimated CdA, Crr, duration, distance, and fit error.

```text
coastdown start 120
coastdown report
roadload start 100
```

### Cold-start and soak model

Cold soak now changes coolant and oil temperatures toward ambient and reports battery-voltage proxy, viscosity multiplier, cranking/after-start enrichment, first-fire state, and oil pressure.

```text
soak 8h
coldstart
quickstart
coldstart
```

### EVAP / fuel-vapor system

The EVAP subsystem tracks purge duty, tank pressure, vapor mass, leak severity, purge valve stuck-open/stuck-closed states, and EVAP DTCs.

```text
evap status
evap purge auto
evap purge on
evap purge off
evap fail leak 0.50
evap fail stuck_open 1.0
evap repair
```

### Catalyst readiness monitors

OBD readiness monitors now progress from warm running and drive-cycle behavior. They include misfire, fuel system, comprehensive components, catalyst, oxygen sensor, EVAP, and EGR/VVT readiness.

```text
readiness
readiness reset
readiness drive_cycle
```

### Plugin architecture

The plugin manager supports concrete runtime plugin loading via manifest files and POSIX native shared-object metadata plugins. Manifest plugins can apply real simulation effects such as torque multipliers and CdA deltas.

```text
plugin list
plugin load plugins/sample_efficiency.plugin
plugin unload
```

Manifest format:

```text
name=sample_efficiency_plugin
description=Manifest plugin that slightly improves torque and aerodynamic drag for testing.
torque_multiplier=1.015
cda_delta=-0.015
fuel_lhv_delta=0.0
```

Native POSIX `.so` plugins can expose optional metadata functions:

```cpp
extern "C" const char* engine_sim_plugin_name();
extern "C" const char* engine_sim_plugin_description();
```

### Regression coverage

The regression suite now covers the added advanced systems at both C++ module level and CLI level.

```bash
cmake -S . -B build
cmake --build build -j
ctest --test-dir build --output-on-failure
```

## Multi-page pinned dashboard

The restored terminal UI now has a multi-page pinned dashboard. The dashboard remains fixed while the simulation loop runs, and `loop start` updates the active page in place without printing scrolling telemetry.

Dashboard pages are organized by subsystem:

```text
main, engine, fuel, ecm, tcm, turbo, cylinders, thermal,
vehicle, obd, emissions, diagnostics, energy, evap, readiness, plugins
```

Interactive controls:

```text
h                    Hide the dashboard only when it is currently shown and the command line is empty.
s                    Show the dashboard only when it is currently hidden and the command line is empty.
Left/Right arrows    Switch dashboard page when the command line is empty.
Left/Right arrows    Edit the current command when text is being typed.
Up/Down arrows       Recall command history.
Ctrl-P/Ctrl-N        Recall previous/next command-history entries.
Ctrl-R               Reverse-search history using the current edit buffer.
Ctrl-A/Ctrl-E        Move to the beginning/end of the command line.
Ctrl-B/Ctrl-F        Move one UTF-8 code point left/right.
Alt-B/Alt-F          Move one word left/right; Ctrl/Alt-arrow variants are accepted.
Ctrl-U/Ctrl-K        Kill text before/after the cursor.
Ctrl-W/Ctrl-Y        Kill the preceding word / yank the most recently killed text.
Ctrl-T               Transpose adjacent UTF-8 code points.
Insert               Toggle insert/overwrite editing mode.
Home/End/Delete      Perform UTF-8-safe line editing.
F2/Ctrl-Space        Open the fuzzy-searchable command palette; Enter executes and Tab inserts.
Tab/Shift-Tab        Open and navigate schema-driven completion; Enter accepts the selected proposal.
Ctrl-Z/Ctrl-_        Undo the most recent edit transaction.
Alt-R                Redo the most recently undone edit transaction.
Bracketed paste      Sanitize pasted control bytes and convert embedded newlines to spaces without execution.
F1                   Toggle the interactive shortcut help overlay.
F6                   Focus Command Activity records; arrows select, Enter/i inspects, and b bookmarks.
/                    Open output-search entry when the command line is empty.
F3/Shift-F3          Select the next/previous output-search match.
Mouse wheel          Scroll the lower Command Activity pane without moving the dashboard.
PageUp/PageDown      Scroll the lower Command Activity pane.
```

Page commands:

```text
page list
page next
page prev
page fuel
page obd
page ecm
page tcm
page turbo
page cylinders
page energy
```

The OBD page displays live decoded Mode 01 data and raw encoded CAN responses. The fuel, ECM, TCM, turbo, cylinder, thermal, vehicle, emissions, diagnostics, energy, EVAP, readiness, and plugin pages expose subsystem-specific real-time state so the dashboard is useful during looped simulation, fault injection, drive cycles, and diagnostic testing.

## Plugin system upgrade: calibration, turbo, fuel, TCM, emissions, dashboard

The simulator now supports typed manifest plugins with concrete simulator effects. Plugins are plain `key=value` files and can be loaded at runtime without recompilation.

### Plugin commands

```text
plugin list
plugin effects
plugin load plugins/calibration_stage1.plugin
plugin load plugins/turbo_is38.plugin
plugin load plugins/fuel_e30.plugin
plugin load plugins/tcm_sport.plugin
plugin load plugins/emissions_highflow.plugin
plugin load plugins/dashboard_research.plugin
plugin unload
```

### Implemented plugin types

- `type=calibration`: adjusts torque, BSFC, VE, EGT, boost, spark/redline metadata.
- `type=turbo`: adjusts compressor/turbine efficiency, boost authority, surge/choke margins, and can load compressor/turbine map CSV files.
- `type=fuel`: adds a full fuel-chemistry overlay including octane, ethanol content, stoichiometric AFR, lower heating value, density, vapor pressure, carbon fraction, charge cooling, and torque effects.
- `type=tcm`: applies a real transmission-control strategy overlay: forced mode, shift RPM offsets, line-pressure delta, clutch-pressure multiplier, shift-time multiplier, torque-reduction multiplier, and TCC lock-speed delta.
- `type=emissions`: applies catalyst/emissions tuning: light-off temperature delta, catalyst efficiency multiplier, CO/HC/NOx/PM multipliers.
- `type=dashboard`: injects live plugin-provided dashboard overlay lines into the pinned dashboard.

### Included sample plugins

```text
plugins/calibration_stage1.plugin
plugins/turbo_is38.plugin
plugins/fuel_e30.plugin
plugins/tcm_sport.plugin
plugins/emissions_highflow.plugin
plugins/dashboard_research.plugin
```

Example smoke workflow:

```text
plugin load plugins/calibration_stage1.plugin
plugin load plugins/turbo_is38.plugin
plugin load plugins/fuel_e30.plugin
plugin load plugins/tcm_sport.plugin
plugin load plugins/emissions_highflow.plugin
plugin load plugins/dashboard_research.plugin
plugin effects
quickstart
step 1.0
metrics
tcm status
turbo status
emissions
```

The plugin manager still preserves earlier generic manifest fields such as `torque_multiplier`, `cda_delta`, and `fuel_lhv_delta`, and POSIX `.so` metadata plugin loading remains available where supported.

## Streamlined task-oriented terminal experience

The complete terminal command surface remains available, while a new metadata-driven experience layer reduces interaction density:

```text
ui home                              # task-oriented home screen
ui profile professional              # presentation-only discovery profile
ui find coolant                      # universal command/workflow/metric search
ui menu open                         # additive beginner menu; F7 or Alt-M also opens it
ui theme set colorblind-safe         # semantic color theme; CLI behavior is unchanged
ui form open throttle                # generated validated percent form
ui workspace save diagnostics-night  # named presentation workspace
ui workflow start diagnostic-scan    # resumable guided workflow
ui dashboard show track-engineer     # persistent custom/factory dashboard
ui drill coolant_c                   # metric drill-down
ui issues                            # unified alert and diagnostic issue center
ui preview reset                     # non-executing impact report
ui state undo                        # restore full serialized simulator state
ui transactions                      # grouped typed command results
ui accessibility ascii-only          # accessible terminal rendering
ui refresh ssh                       # 200 ms dashboard refresh
ui keys profile vim                  # contextual keybinding profile
```

F2/Ctrl-Space searches commands, workflows, dashboards, metrics, settings, and workspaces. F7 or Alt-M opens concise beginner menus while the command prompt remains visible. Menu actions preview ordinary canonical commands; Enter executes through the existing dispatcher and Tab inserts the command into the persistent CLI for review or editing. Discovery profiles never disable commands. Forms and workflows emit ordinary canonical commands. The renderer uses dirty-row patches and viewport-only output materialization; modal overlays and resize events safely force complete redraws. See [`docs/STREAMLINED_UI_EXPERIENCE.md`](docs/STREAMLINED_UI_EXPERIENCE.md).


### Beginner menus, persistent CLI, and semantic color themes

The command line remains the authoritative interface. Beginner menus do not replace it, use a second parser, or bypass command validation. Every menu item stores a canonical command string and routes execution through the same transaction, validation, state-capture, history, logging, and result pipeline used by manually typed commands.

```text
F7 / Alt-M                      Open the beginner menu
ui menu open                    Open it from the CLI
ui menu close                   Close it from the CLI
Enter                           Execute the selected canonical command
Tab                             Insert the selected command into the CLI
Esc                             Close without executing
```

Semantic themes are selected independently of command behavior:

```text
ui theme list
ui theme status
ui theme set professional-dark
ui theme set professional-light
ui theme set high-contrast
ui theme set colorblind-safe
ui theme set monochrome
ui theme set amber-terminal
ui theme set system
```

Themes assign consistent meaning to success, warning, failure, focus, metadata, and informational output. Text labels and symbols remain present, so color is never the only state indicator. `NO_COLOR` disables color emission regardless of the selected theme; accessibility modes can additionally enforce no-color, ASCII-only, high-contrast, or screen-reader rendering.

## Dashboard page-navigation restoration

The pinned terminal dashboard again supports multi-page real-time views. In an interactive POSIX terminal:

- Press the right arrow key with an empty command line to move to the next dashboard page.
- Press the left arrow key with an empty command line to move to the previous dashboard page.
- Left/right arrow editing is preserved while text is present on the command line.
- Use `page list`, `page next`, `page prev`, or `page <name>` for command-driven navigation.

Dashboard pages currently include:

```text
main engine fuel ecm tcm turbo cylinders thermal vehicle obd emissions diagnostics energy evap readiness plugins
```

The pinned dashboard, scrollable lower Command Activity pane, mouse-wheel/PageUp/PageDown scrolling, command history, tab completion, advanced `--help`, plugin overlays, vehicle presets, emissions, CAN/UDS, validation, TCM, turbo, cylinder diagnostics, and all existing simulation commands remain available.

### Dashboard arrow-key navigation fix

Interactive dashboard page navigation is handled directly in the raw terminal input loop:

- `Right Arrow` advances to the next dashboard page when the command line is empty.
- `Left Arrow` moves to the previous dashboard page when the command line is empty.
- When text is being typed, left/right arrows continue to edit the command line normally.
- Supported escape sequences include normal cursor-key CSI sequences, application cursor-key sequences, and modified CSI cursor sequences.
- Command alternatives remain available: `page next`, `page prev`, `page list`, and `page <name>`.

### Dashboard arrow-key regression test

The test suite now includes `dashboard_arrow_pty`, which runs the simulator under a pseudo-terminal and verifies that `Right Arrow` / `Left Arrow` switch dashboard pages while the command line is empty. This guards the multi-page dashboard against future regressions from plugin, shell, or renderer changes.


## Responsive console renderer and dashboard visibility

The interactive POSIX console uses one layout and rendering pipeline for the pinned dashboard, Command Activity viewport, status/footer row, and command prompt.

Dashboard and workspace visibility controls:

```text
h    Hide the dashboard only while it is shown and the command line is empty
s    Show the dashboard only while it is hidden and the command line is empty
F4   Hide/show the complete lower Command Activity pane; the dashboard expands vertically
```

Equivalent lower-pane commands are `ui lowerpane show|hide|toggle|status` and `output pane show|hide|toggle|status`. Dashboard-focus mode preserves output, history, filters, bookmarks, and simulation state. When the lower pane is hidden, printable input or Enter safely restores it before command editing; F6 restores it before entering output focus. The lower-pane state is included in atomic UI preference persistence.

The state-sensitive handling is intentional: while the dashboard is already shown, `s` is ordinary command input, so commands such as `status`, `step`, and `search` can be entered without a prefix or workaround. While the dashboard is hidden, `h` is ordinary command input, so `help` and other `h...` commands work normally.

When hidden, the Command Activity pane expands into the released rows. Showing the dashboard contracts it without discarding output. Live-follow mode remains pinned to the newest record, while historical scrolling remains anchored to the same logical output record.

The renderer provides:

- ANSI-aware terminal display-width calculation.
- UTF-8 validation and code-point-safe truncation.
- Combining-character and wide-character column accounting.
- Width-aware wrapping with continuation indentation.
- Reflow of stored logical output after terminal-width changes.
- `SIGWINCH` handling plus dimension polling for reliable resize detection.
- Typed-command preservation during resize-triggered repaint.
- Responsive `full`, `compact`, `narrow`, and `minimal` dashboard profiles.
- Synchronized dirty-row repaint using terminal synchronized-update markers, with safe full redraws after resize or modal transitions.
- One bounded write path with `EINTR`, `EAGAIN`, and short-write handling.

Density selection is automatic:

| Profile | Default selection |
|---|---|
| `full` | At least 120 columns and 30 rows |
| `compact` | At least 90 columns and 22 rows |
| `narrow` | At least 68 columns and 15 rows |
| `minimal` | Smaller usable terminals |

The profile changes presentation density only. Dashboard pages, commands, options, subsystem access, scrollback, history, tab completion, mouse operation, and simulation behavior remain unchanged.

Regression coverage includes:

```text
dashboard_visibility_pty
dashboard_scroll_anchor_pty
terminal_resize_density_pty
terminal_resize_anchor_pty
terminal_formatting_regression
ui_features_pty
ui_preferences_pty
ui_professional_workflow_pty
ui_input_fuzz_pty
ui_golden_frames
ui_beginner_menu_theme_pty
ui_no_color_pty
lower_pane_visibility_pty
help_focus_pty
user_manual_regression
```

### Interactive status, help, severity, filters, search, and preferences

The dedicated reverse-video status bar is independent of the output footer and command prompt. Its segments are configurable and persisted. Available segments are `mode`, `edit`, `help`, `menu`, `theme`, `loop`, `dashboard`, `page`, `filter`, `search`, `scroll`, `layout`, `validation`, `focus`, `bookmarks`, `watch`, and `status`. The `menu` and `theme` segments are optional so established operational indicators retain priority in the default full-width preset.

```text
ui statusbar segments
ui statusbar segment show|hide|toggle <name>
ui statusbar move <visible-segment> <1..N>
ui statusbar preset full|minimal|operations|diagnostics
ui statusbar on|off|toggle
```

The help system is a focused, modal, multi-topic overlay rendered as part of the same buffered frame; it does not mutate simulation output, command text, or scrollback. `F1`, `Shift-F1`, or `Alt-H` opens it, `Left`/`Right` or `PageUp`/`PageDown` changes topics, `Home`/`End` jumps to the first/last topic, and `Esc`, `Ctrl-G`, or `F1` closes it. Commands are `ui help topics`, `ui help quick|workspace|editing|output|terminal`, `ui help next|prev|first|last`, and `ui help hide`. MuzixDiagSys enables application cursor/keypad mode and terminal focus reporting while active and restores them on exit. If the desktop environment or terminal emulator consumes bare F1 before transmitting it to the PTY, no terminal application can override that global shortcut; use `Shift-F1`, `Alt-H`, or `ui help`, or remove the global F1 binding in the host environment.

The searchable command palette opens with `F2` or `Ctrl-Space`. It fuzzy-matches command names and descriptions, supports Up/Down or Ctrl-P/Ctrl-N selection, executes with Enter, inserts the selected command with Tab, and closes with Esc or Ctrl-G. The beginner menu opens with `F7`, `Alt-M`, or `ui menu open`. Its eight concise categories—Home, Model, Scenario, Run, Monitor, Analyze, Validate, and Help—are additive front ends to the same command dispatcher. Enter executes the selected canonical command; Tab places it in the persistent command editor; Esc closes the menu without changing simulator state. Schema-driven completion uses the same command catalog: Tab opens a candidate overlay containing descriptions, Tab/Shift-Tab selects, and Enter inserts the selected value. The command line is validated continuously for unknown commands, missing arguments, invalid numeric input, and bounded value ranges; incomplete/error diagnostics are rendered inline without executing the command.

The complete console now uses a global root-command registry, a context-sensitive nested grammar, and delegated industrial platform registries shared by execution, aliases, completion, validation, and palette discovery. Every executable root alias, documented nested command, dynamic preset/parameter domain, and industrial vehicle, assurance, electrification, frontier, research, or federation route is available through Tab completion. `command-schema validate` and exhaustive non-interactive plus PTY regressions make future execution/completion drift release-blocking. See `docs/COMMAND_REGISTRY_AND_COMPLETION.md`.

The editor maintains bounded transactional undo and redo histories: `Ctrl-Z` or `Ctrl-_` undoes, and `Alt-R` redoes. Bracketed-paste mode is enabled while the application owns the terminal. Pasted control characters are removed, invalid UTF-8 is replaced safely, CR/LF sequences are converted to spaces, input is capped at 64 KiB, and pasted content is never submitted automatically.

The optional watch panel is a responsive live-metric panel with bounded histories and compact Unicode sparklines:

```text
watch status
watch panel on|off|toggle
watch add <rpm|torque|power|hp|boost|map|lambda|afr|coolant|oil|oil_pressure|egt|speed|acceleration|throttle|fuel_flow|bte>
watch remove <metric>
watch history <8..256>
watch clear
```

Press `F6` to enter output-record focus. Up/Down selects stable logical record IDs; Enter or `i` opens the structured event inspector; `b` toggles a bookmark; Esc/F6 returns to command focus. The inspector shows record ID, originating command ID, severity, subsystem, category, monotonic timestamp, bookmark state, and wrapped message text. Bookmark commands support list, next/previous navigation, deletion, clearing, annotation, and CSV export.

Output is retained as structured logical records with an assigned UI severity: `TRACE`, `DEBUG`, `INFO`, `NOTICE`, `WARNING`, `ERROR`, or `CRITICAL`. The severity is preserved across terminal reflow and is used by filtering and the `ui severity` report. Existing textual output is not removed or rewritten.

Filtering and search commands:

```text
filter status
filter severity all|debug|info|notice|warning|error|critical
filter text <substring>
filter case on|off
filter expr <field-expression>
filter clear
search <substring>
search next
search prev
search clear
ui filter ...
ui search ...
```

Filtering changes only which stored logical records are rendered; it does not discard scrollback. Structured expressions support parentheses, `and`/`or`/`not`, comparison operators, `contains`, `startswith`, `endswith`, and `in {…}` over `id`, `command_id`, `timestamp_ms`, `severity`, `subsystem`, `category`, `message`, and `bookmarked`. Expressions are limited to 4096 bytes, 256 tokens, and 16 nesting levels, compile transactionally, and report exact error columns. Search operates on the currently filtered, reflowed output, wraps at the ends, scrolls the selected match into view, and marks it with `▶`. Pressing `/` on an empty command line opens search-entry mode; `F3` and `Shift-F3` navigate matches.

UI preferences are loaded transactionally and saved atomically using a temporary file followed by rename. Persisted fields include dashboard visibility, status-bar visibility and segment order, active dashboard page, minimum severity, text and structured field filters, filter case sensitivity, watch-panel visibility, watch metrics, watch-history length, and the active semantic color theme. Search text, bookmarks, modal overlays, and editor undo state are deliberately session-local.

Preference location precedence:

1. `MUZIXDIAGSYS_UI_PREFS` when set to a non-empty explicit path (legacy `AESIM_UI_PREFS` is also accepted).
2. `$XDG_CONFIG_HOME/muzixdiagsys/ui_preferences.conf`.
3. `$HOME/.config/muzixdiagsys/ui_preferences.conf`.
4. `.muzixdiagsys_ui_preferences` when no home/config directory is available; `.engine_sim_ui_preferences` is read as a legacy fallback.

Set `MUZIXDIAGSYS_UI_PREFS_DISABLE=1` or set `MUZIXDIAGSYS_UI_PREFS` to an empty value to disable persistence. The historical `AESIM_UI_PREFS_DISABLE` and `AESIM_UI_PREFS` aliases remain accepted. Files larger than 64 KiB, unknown keys, malformed values, and malformed records are rejected without partially applying settings; defaults remain active and the diagnostic is reported in the UI. Use `ui prefs show`, `ui prefs save`, or `ui prefs reset` to inspect or manage the stored state.

These tests validate dashboard expansion/contraction, UTF-8 integrity, ANSI-aware line widths, automatic resize repaint, all density transitions, typed-input retention, logical scroll anchoring, and full-frame synchronization.

## Drivetrain launch / throttle response fix

The simulator now includes an explicit low-speed automatic-launch coupling model so vehicle speed increases correctly when throttle is raised in drive conditions. The model adds torque-converter creep/stall launch torque at very low road speed, instead of requiring unrealistically high throttle to overcome rolling resistance from rest.

New and updated commands:

```text
throttle <0..1|0..100>
throttle up [delta]
throttle down [delta]
drivecheck
drivetrain
key off|run|start
start
shutdown
```

Notes:

- `throttle up` and `throttle down` adjust throttle in percentage-point style increments. The default increment is 10 percentage points.
- If the simulation loop is stopped, changing throttle changes the command but speed will not change until `loop start` or `step <seconds>` advances the model.
- `drivecheck` reports why the vehicle is or is not accelerating, including loop stopped, ignition off, neutral gear, clutch disengaged, brake applied, or insufficient breakaway tractive force.
- The main dashboard and `status` output now include drive-readiness diagnostics.

Regression coverage now includes a drivetrain launch test that runs `quickstart`, `throttle up`, advances the simulation, and asserts that road speed increases from rest.

## Automatic WOT shift fix

The automatic transmission control logic now includes a WOT-specific shift schedule and kickdown lockout hysteresis:

- `throttle 100` in `mode automatic` no longer hunts between gears 1 and 2.
- Full-throttle acceleration now progressively shifts through the forward ratios and reaches gear 6 as road speed increases.
- Kickdown requests are suppressed when the lower gear would land too close to the upshift / redline region.
- The legacy automatic shift fallback and the full TCM now use the same anti-hunt behavior.

Regression coverage:

```bash
ctest --test-dir build --output-on-failure
```

Includes `automatic_wot_shift_regression`, which verifies:

```text
quickstart
mode automatic
throttle 100
step 20.0
status
```

reaches gear 6 without reintroducing 1/2 hunting.

## Automatic high-load shift hysteresis fix

The automatic transmission controller now treats near-wide-open throttle as a high-load speed-scheduled regime with a real hysteresis band instead of allowing an immediate kickdown/upshift loop.

Fixes included:

- `throttle 95` after a WOT pull no longer bounces between adjacent upper gears such as 4 and 5.
- The TCM is now the sole automatic shift scheduler; the older gearbox-local automatic scheduler is bypassed during automatic operation to prevent competing shift decisions.
- Transmission shift timers are decremented by the main simulation loop so the TCM can continue progressing through gears after each shift.
- High-load upshifts use gear-dependent road-speed thresholds.
- High-load downshifts use lower gear-dependent thresholds with a deadband so a downshift cannot immediately trigger the matching upshift.
- A post-shift anti-hunt timer prevents rapid reversal of the last shift.

Regression coverage now includes `automatic_high_load_hysteresis_regression`, which runs:

```text
quickstart
mode automatic
throttle 100
step 20.0
throttle 95
step/status repeated
```

and verifies that the gearbox holds a stable high gear without a 4/5 hunting signature.

## Automatic coastdown downshift fix

The automatic transmission controller now includes a dedicated light-throttle / closed-throttle coastdown schedule. This fixes the case where the gearbox would reach gear 6 during a WOT pull but then remain stuck in 6th as speed and RPM decayed after throttle reduction.

Fixes included:

- Closed-throttle coastdown now uses gear-dependent road-speed downshift thresholds.
- The TCM downshifts from 6th as vehicle speed falls instead of lugging the engine down toward idle in top gear.
- Continued deceleration progressively downshifts through the lower gears.
- The existing high-load anti-hunt logic remains intact, so the 4/5 hunting fix is preserved.
- Downshifts are guarded by projected lower-gear RPM checks to avoid mechanically impossible or redline-adjacent shifts.

Regression coverage now includes `automatic_coastdown_downshift_regression`, which runs:

```text
quickstart
mode automatic
throttle 100
step 20.0
throttle 0
step/status repeated
```

and verifies that the transmission leaves gear 6 during coastdown and continues downshifting as speed decreases.

## RPM display and tachometer guardrail update

RPM metrics are now constrained to a four-digit tachometer presentation across the dashboard, status output, dyno/validation summaries, and OBD decoded text. The simulator clamps internal engine RPM to `9999` for user-facing tachometer consistency, and `engine.redline_rpm` is bounded to a maximum applied value of `9500` RPM so transient overshoot cannot produce five-digit RPM metrics.

Regression coverage includes `rpm_four_digit_regression`, which exercises high-throttle operation, `status`, `metrics`, `obd pid 010C`, and `dyno` output and fails if any RPM metric renders as five or more digits.

## Plugin loader path-resolution fix

The plugin loader now resolves manifest and native plugin paths against multiple stable locations instead of only the current working directory. This fixes failures when launching the simulator from `build/`, from the project root, or from another working directory.

Resolved search locations include:

- the exact path supplied by the user
- the current working directory
- parent directories of the current working directory
- the executable directory
- parent directories of the executable directory
- the loaded plugin manifest directory for secondary assets such as turbo compressor/turbine maps
- the project root inferred from the plugin manifest location

Example workflows that now work:

```text
cd MuzixDiagSys
./build/muzixdiagsys
plugin load plugins/calibration_stage1.plugin
plugin load plugins/turbo_is38.plugin
plugin effects
```

```text
cd MuzixDiagSys/build
./muzixdiagsys
plugin load plugins/calibration_stage1.plugin
plugin load plugins/turbo_is38.plugin
plugin effects
```

The regression suite includes `plugin_loader_regression`, which launches the simulator from the build directory and verifies that calibration, turbo, fuel, TCM, emissions, and dashboard plugins all load and apply correctly.

## Plugin dashboard visibility fix

Loaded plugins now appear directly on the pinned dashboard, not only in `plugin effects` output. The main dashboard page shows a `Plugin stack` line and a `Plugin effect` line whenever one or more plugins are loaded. The `plugins` dashboard page still shows expanded plugin/dashboard overlay lines. This preserves the existing plugin commands while making plugin state visible during real-time monitoring.

Example:

```text
plugin load plugins/calibration_stage1.plugin
plugin load plugins/turbo_is38.plugin
plugin load plugins/fuel_e30.plugin
plugin load plugins/tcm_sport.plugin
plugin load plugins/emissions_highflow.plugin
plugin load plugins/dashboard_research.plugin
metrics
page plugins
```

Regression coverage: `plugin_dashboard_regression` verifies that loaded plugins appear on dashboard output.

## Real-world expanded vehicle and engine presets

This build adds source-anchored presets for General Motors, Ford, Audi, and Volkswagen. These presets use public horsepower/torque/displacement/geometry/ratio anchors where available and generate simulator calibration maps around those anchors; they are not proprietary OEM ECU calibrations.

New engine commands:

```text
engines
engine list
engine status
engine vw_golf_r_2.0_tsi_ea888_evo4
engine audi_rs3_2.5_tfsi
engine audi_s4_3.0_tfsi
engine ford_mustang_gt_5.0_coyote
engine ford_f150_3.5_ecoboost
engine gm_corvette_c8_lt2
engine gm_camaro_ss_lt1
engine gm_camaro_zl1_lt4
```

New vehicle presets include:

```text
vehicle vw_golf_r_mk8_dsg
vehicle audi_s3_8y
vehicle audi_rs3_8y
vehicle audi_s4_b9
vehicle ford_mustang_gt_s650_manual
vehicle ford_mustang_gt_s650_auto
vehicle ford_f150_3.5_ecoboost_10at
vehicle gm_corvette_c8_stingray
vehicle gm_camaro_ss_6mt
vehicle gm_camaro_zl1_10at
```

Recommended paired workflows:

```text
engine ford_mustang_gt_5.0_coyote
vehicle ford_mustang_gt_s650_manual
quickstart
mode automatic
throttle 100
step 10
dyno

engine gm_corvette_c8_lt2
vehicle gm_corvette_c8_stingray
dyno

engine audi_rs3_2.5_tfsi
vehicle audi_rs3_8y
cycle run urban
```

The regression suite includes an `expanded_realworld_presets_regression` test that validates these presets load, pair with vehicle configurations, run a dyno sweep, and preserve four-digit RPM output.

## Dashboard metric dictionary

The simulator now includes a searchable dictionary for every parameter and metric displayed on the pinned dashboard, including header fields, all dashboard pages, OBD PID labels, EVAP/readiness candidate labels, plugin overlay labels, and repeated subsystem labels.

Commands:

```text
dict                         In the interactive pinned dashboard UI, open the dictionary search prompt.
dict <parameter-or-metric>    Search by displayed label or alias.
dict list                    List every dictionary label.
dict page <name>              List dictionary labels for one dashboard page.
```

Examples:

```text
dict rpm
dict lambda
dict pressure ratio
dict wheel force
dict page engine
```

Each dictionary response reports the dashboard page(s), units/display format, detailed meaning, interpretation guidance, model source, and supported aliases. Tab completion includes the `dict` command and dictionary search terms.

Regression coverage: `metric_dictionary_regression` verifies that dictionary lookups return detailed descriptions and that representative labels from all dashboard areas are listed.


## Research Expansion: Batch, Monte Carlo, Telemetry, Fitting, and Aftertreatment

This build adds executable research workflows on top of the existing interactive simulator.

### Deterministic batch runner

Run a line-oriented manifest where each non-comment line is a simulator action:

```text
batch run data/batch_example.txt data/batch_results.csv
```

Supported manifest actions include `reset`, `quickstart`, `step <seconds>`, `throttle <pct>`, `brake <pct>`, `fuel <name>`, `vehicle <preset>`, `engine <preset>`, `mode <manual|automatic>`, and `gear <n>`.
The optional CSV output records time, RPM, torque, power, speed, MAP, lambda, and catalyst efficiency after every manifest action.

### Deterministic Monte Carlo expansion

```text
montecarlo 100 data/mc_results.csv
```

The Monte Carlo runner uses a fixed seed and varies vehicle mass, CdA, rolling resistance, ambient temperature, and throttle. It exports peak torque, final speed, fuel use, CO2, and NOx per trial.

### External telemetry importer and comparator

```text
telemetry import data/sample_telemetry.csv
telemetry compare
telemetry replay 2.0
telemetry export-residuals data/residuals.csv
```

The importer accepts timestamped CSV data with columns such as `time`, `throttle`, `brake`, `rpm`, `speed`, `torque`, `map`, `boost`, `lambda`, `fuel_flow`, and `coolant`. The comparator applies control columns to the simulator and reports residual bias, MAE, and RMSE for matching measured metrics.

### Calibration fitting / parameter estimation

```text
fit status
fit dyno data/sample_dyno.csv 18
fit telemetry 12
```

`fit dyno` estimates an executable torque scale against measured RPM/torque points. `fit telemetry` estimates torque, boost, fuel-flow, and lambda correction factors from the loaded telemetry table. These fitted parameters are applied directly in the simulation loop until `reset` is used.

### Advanced aftertreatment / emissions chemistry

The emissions model now includes oxygen-storage dynamics, aging factor, CO/HC/NOx conversion fractions, catalyst exotherm, upstream/downstream oxygen sensor voltages, and NOx storage fraction. These states are updated every simulation step and appear in the `emissions` report and emissions CSV export.

## Professional platform expansion: scenarios, schemas, studies, real-time, FMI, DBC, and ECU strategy

This build adds executable professional-platform features while preserving the existing dashboard, dictionary, tracing, combustion, turbo, air-path, thermal, sensor/actuator, CAN, telemetry, fitting, batch, and Monte Carlo features.

### Scenario manifests

Formal YAML and JSON experiment manifests can now drive deterministic simulator workflows:

```text
scenario validate data/scenario_example.yaml
scenario run data/scenario_example.yaml studies/scenario_run
scenario template data/new_scenario.yaml yaml
scenario template data/new_scenario.json json
```

Scenario commands are validated and executed in order. Supported scenario operations include reset, quickstart, step, throttle, brake, clutch, fuel, engine, vehicle, mode, gear, telemetry import/compare/replay, fit dyno/telemetry, emissions export, DBC export/import, FMI export, ECU commands, and plugin loading.

### Schema validation

The simulator now performs formal file validation for the major file families used by the project:

```text
schema validate data/scenario_example.yaml
schema validate plugins/calibration_stage1.plugin
schema validate data/sample_telemetry.csv
schema validate configs/powertrain_catalog.yaml powertrain_catalog
schema dump scenario
schema dump plugin
schema dump telemetry
schema dump calibration
schema dump vehicle
```

Validation reports include pass/warn/fail counts, required-field checks, recognized-channel checks, plausibility bounds, and command-support checks.

### Study packages

A complete study package can be generated from a scenario:

```text
study run data/scenario_example.yaml studies/example_study
```

Generated packages include report.md, summary.json, session_report.md, scenario_trace.csv, emissions.csv, telemetry_residuals.csv, generated_can.dbc, and muzixdiagsys_model.fmu.

### Real-time deterministic mode

The background integration loop now supports deterministic real-time scheduling controls:

```text
realtime on
realtime rate 1.0
realtime dt 0.01
realtime status
realtime off
```

The status report tracks fixed dt, target rate, effective wall-clock period, update count, mean update time, and deadline misses.

### FMI/FMU export and co-simulation

The simulator can export a valid stored-zip FMU-style package containing modelDescription.xml, resources/aesim_state.json, documentation, and reference C source. The same executable can load that FMU package and run a deterministic co-simulation trace:

```text
fmi export muzixdiagsys_model.fmu
fmi cosim muzixdiagsys_model.fmu 2.0 fmi_trace.csv
fmi status
```

The FMU artifact is a real ZIP container and is suitable for inspection or downstream build-system integration. The built-in `fmi cosim` command validates the package and runs the simulator as the co-simulation engine.

### DBC import/export and CAN signal modeling

DBC support maps simulator metrics to CAN signals and can round-trip generated DBC files:

```text
dbc export muzixdiagsys_generated.dbc
dbc import muzixdiagsys_generated.dbc
dbc signals
can dbc export muzixdiagsys_generated.dbc
can dbc import muzixdiagsys_generated.dbc
```

The DBC signal report shows current physical values for engine speed, torque, MAP, boost, lambda, vehicle speed, gear, coolant temperature, oil pressure, and catalyst temperature.

### ECU control-strategy model

A real executable ECU strategy layer is available without changing legacy/default simulator behavior. The default `stock` mode is observational so legacy regressions remain stable. Explicit ECU modes enable closed-loop control effects:

```text
ecu status
ecu mode closed_loop
ecu mode sport
ecu target lambda 0.92
ecu target boost 155
ecu target torque 360
ecu knock on
ecu reset
```

The ECU layer performs lambda target correction, boost limiting, torque limiting, knock retard, and limp-mode activation under selected active strategies.

## Human-readable terminal presentation

Interactive and batch-facing text output now use a shared terminal presentation layer. Existing commands and script-readable metric labels remain available, while human-facing output is grouped and aligned consistently.

Key presentation changes:

- `status` is divided into engine, fuel/combustion, thermal/lubrication, transmission/vehicle, geometry, and drive-readiness sections.
- `help` uses aligned command/description columns, continuation indentation, and full-width treatment for long research command families.
- `params` uses a compact two-column parameter list.
- Interactive Command Activity output is prefixed with the command that produced it.
- Traditional report headings followed by dashed rules are converted into bordered terminal sections in the interactive Command Activity pane.
- Dense subsystem lines containing multiple `key=value` fields are expanded into labeled rows.
- Usage, error, warning, and successful completion messages receive consistent status badges.
- Scrollback wrapping is word-aware and preserves indentation instead of splitting text at arbitrary character positions.
- Stable labels such as `RPM:`, `Mode: ... | gear:`, `Speed:`, and `Drive readiness:` are preserved for scripts and existing regression consumers.

The `terminal_formatting_regression` CTest target validates both non-interactive output and the live pseudo-terminal presentation path.

## 2026-07-09 Modular research-core implementation

This build adds a compiled, independently testable `aesim_core` library while preserving every established simulator feature and command family. The new core supplies a deterministic integer-nanosecond multi-rate scheduler, per-cylinder crank-angle combustion, dynamic intake/exhaust/turbo gas-path physics, statistical validation, uncertainty quantification, hybrid parameter estimation, and cryptographically verifiable experiment provenance.

### Build

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=RelWithDebInfo
cmake --build build --parallel
ctest --test-dir build --output-on-failure
```

### Modular core and cylinder trace

```text
core status
core coupling 0.65
core period gas_path 0.001
core period combustion 0.005
core period diagnostics 0.010
step 2.0
core export reports/research_core_state.json
core trace reports/cylinder_resolved_trace.csv
```

The coupling value is a migration-safe blend. `0.0` retains the established plant output, while `1.0` applies the modular core at full weight. Disabling the core does not disable any legacy subsystem.

### Formal validation

```text
validation research run data/research_validation_reference.csv reports/formal_validation.md
validation research status
```

Dataset columns use `observed.<metric>` and optional `sigma.<metric>` names. Reports include bias, MAE, RMSE, normalized RMSE, maximum error, residual deviation, R², confidence intervals, residual autocorrelation, reduced chi-square, and explicit requirement pass/fail results.

The bundled reference CSV is a deterministic software-regression dataset generated by `research_reference_generator`; it is not independent physical evidence. Use traceable measured data for scientific or product validation.

### Uncertainty and sensitivity

```text
uncertainty research run 128 2748 reports/research_uq.csv
uncertainty research sobol 64 2748 reports/research_sobol.json
uncertainty research status
```

The implementation provides deterministic Latin-hypercube sampling, configurable probability distributions, quantiles and confidence intervals, Pearson and standardized-regression sensitivities, and first/total-order Sobol indices.

### Parameter estimation

```text
calibrate research fit data/research_validation_reference.csv 8 reports/research_calibration.json
calibrate research status
```

Calibration combines bounded Differential Evolution with Levenberg-Marquardt refinement, robust Huber residuals, covariance/standard-error estimation, parameter correlations, and automatic application of the fitted values to the live modular core.

### Reproducible experiments

```text
experiment begin baseline experiments 7348921
experiment event protocol "warm-up complete"
step 5.0
core export reports/core_state.json
experiment artifact reports/core_state.json core-state
validation research run data/research_validation_reference.csv reports/validation.md
experiment artifact reports/validation.md validation
experiment end
experiment verify experiments/<run-directory>
```

Each experiment records canonical configuration and executable identities, UTC lifecycle metadata, deterministic seed, environment information, telemetry, events, summary values, artifact sizes, and SHA-256 hashes in a JSON manifest. External artifacts and the executing binary are copied into a content-addressed, run-relative package, allowing the finalized run directory to be relocated and verified independently of the original paths.

See `docs/RESEARCH_CORE_ARCHITECTURE.md` for model equations, architecture, dataset schema, command semantics, validation interpretation, and sanitizer instructions.

## Industrial HIL, Automotive Networks, Measurement, and Verification Platform

The simulator includes an additive `aesim_industrial` C++17 library. Existing
engine, research-core, professional-platform, CLI, plugin, FMI, dashboard, and
file-format features remain available. The industrial layer exposes the live
plant through typed signals and provides deterministic testbench services.

### Hard real-time and HIL execution

The Linux runtime supports memory locking, stack prefaulting, CPU affinity,
`SCHED_FIFO`, absolute `CLOCK_MONOTONIC` release sleeps, execution/slack
statistics, warning thresholds, deadline detection, and count/skip/stop overrun
policies. Strict mode makes unavailable privileges or facilities fatal instead
of silently degrading. Actual hard-deadline qualification still depends on the
kernel, drivers, firmware, I/O hardware, CPU isolation, and system deployment.

```text
industrial hil status
industrial hil strict on|off
industrial hil period <microseconds>
industrial hil warning <microseconds>
industrial hil priority <1..99>
industrial hil affinity <cpu...>
industrial hil policy count|skip|stop
industrial hil io loopback
industrial hil io udp <local-address> <local-port> <remote-address> <remote-port>
industrial hil io open|close|safe
industrial hil on|off
```

HIL channels include analog voltage/current, digital, PWM, frequency, encoder,
and thermocouple abstractions. Every channel has direction, range, unit,
quality, timestamp, and safe-state metadata. A bounded binary UDP backend and a
deterministic loopback backend are included.

### SocketCAN, CAN FD, ISO-TP, UDS, and J1939

On Linux, SocketCAN uses native CAN/CAN-FD frames and interface error handling.
The loopback transport provides deterministic tests without physical hardware.
ISO-TP supports single, first, consecutive, and flow-control frames with block
size, sequence, timeout, and payload limits. The UDS virtual ECU implements
session control, reset, DTC read/clear, DID read/write, security access,
communication control, tester present, routine control, and transfer services.
The J1939 stack includes 29-bit identifiers, address claim, single-frame PGNs,
BAM transport, and DM1/DM2 diagnostic messages.

```text
industrial network loopback
industrial network socketcan can0
industrial network open
industrial network send 0x321 01 02 03 04 05 06 07 08 09
industrial network receive 100
industrial network uds 10 03
industrial network dtc set 0x0299 underboost
industrial network j1939 claim
industrial network j1939 dm1
industrial network close
```

### XCP and generated A2L

The UDP XCP server implements command/response transport, MTA upload/download,
calibration pages, checksum, DAQ allocation/configuration, event sampling, and
DTO publication to the active peer. The A2L generator derives measurements,
characteristics, data types, ranges, units, addresses, conversions, record
layouts, groups, and XCP transport metadata directly from the typed signal
registry.

```text
industrial xcp start 127.0.0.1 5555
industrial xcp status
industrial xcp a2l reports/aesim.a2l MUZIXDIAGSYS_PROJECT
industrial xcp cto FF 00
industrial xcp stop
```

### MDF 4.10 measurement recording

The recorder writes an MDF 4.10 binary hierarchy with identification, header,
file-history, data-group, channel-group, channel, conversion, source,
text/metadata, data, and data-list blocks. Channel samples are time aligned,
unit described, and linked to experiment metadata. A structural validator
checks signatures, version, links, block sizes, and bounds.

```text
industrial mdf start reports/run.mf4 0.001 engine.rpm engine.torque_nm combustion.lambda
step 1.0
industrial mdf stop
industrial mdf validate reports/run.mf4
```

### ASAM XIL-compatible automation profile

The XIL testbench provides model-access, network, diagnostic, and electrical
error ports over the simulator's live services. YAML/JSON tests support signal
writes, waits, assertions, commands, CAN-FD frames, UDS requests, fault
injection/clearing, MDF recording, and bounded wait-until actions.

```text
industrial xil run data/industrial_xil_test.yaml reports/xil_result.json
```

This is an operational XIL-compatible automation profile; no third-party ASAM
conformance certification is claimed.

### SSP 2.x and multi-FMU orchestration

The SSP implementation packages and reads `SystemStructure.ssd`, embedded FMUs,
connectors, connections, parameters, and resources in ZIP/Deflate containers.
The orchestration master instantiates FMI 3 components and supports Jacobi,
Gauss-Seidel, and iterative Gauss-Seidel coupling with state rollback,
convergence limits, residual reporting, parameter application, and unit-aware
connection validation.

```text
fmi3 export reports/powertrain.fmu
industrial ssp export reports/powertrain.ssp reports/powertrain.fmu PowertrainSystem
industrial ssp inspect reports/powertrain.ssp
industrial ssp load reports/powertrain.ssp
industrial ssp algorithm iterative_gauss_seidel 12 1e-8
industrial ssp initialize 0
industrial ssp set Powertrain throttle 0.5
industrial ssp step 0.01
industrial ssp get Powertrain rpm
industrial ssp unload
```

The implementation is an operational SSP 2.x profile and is not represented as
external standards-body certification.

### Requirements, tests, and evidence

The traceability repository links versioned requirements, test definitions, and
immutable evidence records. Evidence contains requirement/test content hashes,
artifact SHA-256, verdict, timestamp, run identifier, and metrics. Coverage
reports detect uncovered requirements, failures, stale evidence after source
definition changes, and orphan tests.

```text
industrial requirements load-requirements data/industrial_requirements.yaml
industrial requirements load-tests data/industrial_tests.yaml
industrial requirements evidence TEST-HIL-RT-001 REQ-HIL-RT-001 PASS reports/run.mf4 run-001
industrial requirements coverage
industrial requirements matrix reports/traceability.md
industrial requirements save reports/traceability.json
```

### Automated fault campaigns

Fault manifests can contain explicit cases and Cartesian matrices. Every case
resets and preconditions the plant, clears/re-baselines diagnostic state,
injects a timed fault, evaluates safety expressions, measures DTC detection and
safe-state latency, checks DTC classification, records unexpected DTCs as false
positives, clears the fault, and writes JSON, Markdown, and CSV reports.

```text
industrial campaign template reports/campaign.yaml
industrial campaign run data/industrial_fault_campaign.yaml reports/campaign
industrial campaign report
```

Example manifests are provided in:

```text
data/industrial_xil_test.yaml
data/industrial_requirements.yaml
data/industrial_tests.yaml
data/industrial_fault_campaign.yaml
```

## Virtual vehicle and distributed validation platform

The simulator now includes an additive `aesim::vehicle` subsystem providing:

- OpenDRIVE road import, geometry sampling, lane positioning, nearest-road lookup,
  and graph routing.
- Deterministic OpenSCENARIO execution and OSI-style vehicle-world interchange.
- Four-wheel vehicle, tire, ABS/brake, regenerative-braking, and environment
  dynamics.
- Uptane-oriented signed metadata verification with persistent A/B activation,
  health acceptance, rollback, and recovery.
- gPTP clock synchronization and deterministic TSN gate-window synthesis.
- COVESA VSS signal normalization and VISS read/write/subscription services.
- Formal supplier-artifact qualification profiles.
- Deterministic local and TCP-distributed parameter studies.

```text
industrial vehicle status
industrial vehicle map load data/vehicle_world.xodr
industrial vehicle scenario load data/vehicle_world.xosc
industrial vehicle scenario run 10 0.01
industrial vehicle dynamics configure data/vehicle_dynamics.yaml
industrial vehicle tsn load data/vehicle_tsn.yaml
industrial vehicle tsn synthesize
industrial vehicle vss load data/vehicle_vss.yaml
industrial vehicle study local data/vehicle_study.yaml reports/study.json 8
```

A standalone remote worker is built as:

```text
./build/aesim_study_worker 0.0.0.0 47000
```

Complete architecture, command, validation, and scope documentation is available
in `docs/virtual_vehicle_platform.md`.

## Electrification and multi-domain platform

The simulator includes a modular electrification layer covering electrothermal battery aging, electric drives and hybrid topology composition, Plug & Charge and OCPP charging workflows, coupled heat-pump/HVAC thermal management, acausal equation execution, DDS/ROS-oriented middleware, ISO 23150 sensor fusion, heterogeneous compute backends, and native ONNX inference with runtime safety envelopes.

See [`docs/electrification_multidomain_platform.md`](docs/electrification_multidomain_platform.md) for architecture, commands, configuration examples, and interoperability scope.

## Digital thread and frontier assurance platform

MuzixDiagSys includes an additive frontier layer for SysML v2-oriented and ReqIF digital-thread exchange, ISO/PAS 8800-oriented AI assurance, cryptographically protected V2X and roadside infrastructure, OpenMATERIAL/OpenLABEL/OpenODD asset management, ODD coverage and scenario synthesis, battery thermal-runaway propagation, mixed-criticality virtual ECU/WCET analysis, and differentiable simulation.

See [`docs/digital_thread_frontier_platform.md`](docs/digital_thread_frontier_platform.md) for architecture, supported profiles, command reference, data formats, and validation scope.

```text
industrial frontier status
industrial frontier sysml import data/frontier_system.sysml
industrial frontier reqif import data/frontier_requirements.reqif
industrial frontier ai-safety load data/frontier_ai_safety.yaml
industrial frontier v2x rsu load data/frontier_rsu.yaml
industrial frontier openx material import data/frontier_material.json
industrial frontier odd configure data/frontier_openodd.yaml
industrial frontier runaway configure data/frontier_runaway.yaml
industrial frontier vecu load data/frontier_vecu.yaml
industrial frontier diff load data/frontier_differentiable.yaml
```

## Research integration, digital-twin, and reproducibility platform

The additive `aesim::research2` layer provides partitioned multiphysics
coupling, native OSI protobuf records, online digital-twin estimation,
multi-fidelity Bayesian calibration, formal hybrid reachability, governed
surrogate and POD reduced-order models, deterministic numerical profiles,
OpenTelemetry/eBPF observability, and signed CycloneDX/provenance artifacts.

```text
industrial research2 status
industrial research2 coupling demo 0.01
industrial research2 osi generate reports/ground_truth.osi
industrial research2 estimate demo
industrial research2 bayes demo reports/posterior.json
industrial research2 reach demo reports/counterexample.json
industrial research2 surrogate demo reports/surrogate-registry
industrial research2 numerics strict 1234
industrial research2 observe export reports/traces.otlp.json
industrial research2 attest generate reports/attestation ./build/muzixdiagsys
```

The preCICE adapter loads the actual preCICE C API dynamically, allowing a
standard build to remain independent of a particular preCICE installation. The
wire-compatible OSI profile is documented in
`schemas/osi3/aesim_osi_groundtruth_profile.proto`.

Complete architecture, command, validation, and deployment guidance is in
[`docs/research_integration_platform.md`](docs/research_integration_platform.md).


### Real-world preset selection and transmission stability

`engine list` and `vehicle list` now present each full display name, canonical preset key, public-data basis, and an exact copyable `Select with:` command. The added Toyota GR Corolla, Honda Civic Type R, BMW M3 Competition, Mazda MX-5, Ram Hurricane H/O, Chevrolet Duramax, Porsche 911 Carrera, and Subaru WRX engine/vehicle families are documented in [`docs/REAL_WORLD_PRESET_SOURCES.md`](docs/REAL_WORLD_PRESET_SOURCES.md).

The automatic TCM uses projected adjacent-gear RPM, candidate dwell, post-shift temporal inhibit, spatial hysteresis, and separate high-load/coastdown schedules to prevent steady-throttle adjacent-gear hunting while preserving redline protection, WOT upshifts, kickdown, and coastdown downshifts. Use `tcm status` to inspect the shift reason, pending gear, dwell, and remaining anti-hunt inhibit.

The operator-supplied `--advanced-help` capture incorporated into the manual is retained verbatim at [`docs/advanced_help_flag_reference_2026-07-11.txt`](docs/advanced_help_flag_reference_2026-07-11.txt).

## 2026-07-11 realism, dashboard, and completion update

The driver `throttle` command now represents accelerator-pedal demand rather than a direct percentage of peak engine power. Each vehicle preset carries road-load, rotating-mass, accessory-load, wheelbase/CG, half-pedal equilibrium, and governed-speed calibration; each engine preset contributes rated power/torque and speed anchors. The longitudinal model includes signed aerodynamic drag, speed-dependent rolling resistance, grade, accessory power, load-dependent driveline efficiency, reflected inertia, and jerk-limited acceleration. Use `status` or the `vehicle` dashboard page to inspect effective driver demand, pedal-speed target, wheel/road-load power, effective mass, rolling coefficient, driveline efficiency, and limiter factor.

The dashboard retains all prior pages and metrics but now presents full engine/vehicle identities, explicit label/value separators, section headings, SI/US speed, motion/jerk, and realism diagnostics. The schema-completion popup is a scrolling viewport: Tab/Shift-Tab, arrows, PageUp/PageDown, Home/End, and the mouse wheel keep the selected candidate visible and repaint across viewport boundaries.

See `docs/MUZIXDIAGSYS_USER_MANUAL.md`, sections 3.6, 4.7, and 6.12, for complete operating and validation guidance.

## 2026-07-11 coupled closed-loop vehicle-realism package

Detailed implementation and validation evidence: [`reports/COUPLED_REALISM_IMPLEMENTATION_VALIDATION_2026-07-11.md`](reports/COUPLED_REALISM_IMPLEMENTATION_VALIDATION_2026-07-11.md).

This build couples the driver, engine, transmission, converter, tires, chassis, fuel system, standardized cycles, calibration, uncertainty, and energy accounting inside the live integration step. Existing commands and compatibility behavior remain available.

### Closed-loop virtual driver

```text
driver status|on|off|reset
driver target <km/h>
driver profile cautious|normal|aggressive|economy|track|towing
```

The driver uses reaction filtering, acceleration feed-forward, PID feedback, anti-windup, jerk limiting, actuator slew limits, preview-gated propulsion, explicit overspeed braking, and mutually exclusive throttle/brake arbitration.

### Full engine operating maps

```text
engine map status
engine map torque|bsfc|ve|egt|mfb50 [output.csv]
```

Every engine preset owns bounded RPM/load maps for torque, BSFC, volumetric efficiency, EGT, and MFB50. Full-load public ratings anchor the maps; intermediate cells are engineering reconstructions unless a measured map is explicitly provided.

### Vehicle-specific transmission, converter, and shift dynamics

```text
tcm status
tcm map [output.csv]
tcm lockup auto|force_on|force_off
```

The active preset generates its own shift schedule. The hydrodynamic converter models speed ratio, torque ratio, capacity factor, efficiency, lockup slip, heat, and fluid temperature. Accepted shifts execute fill, torque, inertia, and completion phases with clutch pressure, slip, torque capacity, and accumulated shift energy.

### Four-wheel tire-slip plant

All four wheels retain independent angular speed, longitudinal slip, normal load, drive/brake torque, force, temperature, and dissipated energy. FWD/RWD/AWD/4WD torque distribution, front brake bias, traction control, ABS, tire-force relaxation, and bounded low-speed substeps are coupled to chassis acceleration.

### EPA/WLTP tracking validation

```text
cycle list
cycle validate ftp75 [trace.csv]
cycle validate hwyfet [trace.csv]
cycle validate us06 [trace.csv]
cycle validate wltc3a [trace.csv]
cycle validate wltc3b [trace.csv]
```

Reports include MAE, RMSE, P95/max error, distance error, timing-window compliance, fuel, CO2, shifts, and a PASS/MARGINAL/FAIL engineering-screening grade. Results are not legal certification or homologation.

Final release-validation results for the default calibrated sedan are HWFET PASS (0.259 km/h RMSE), FTP-75 PASS (0.433 km/h), WLTC Class 3b PASS (0.497 km/h), and US06 MARGINAL (2.444 km/h). Absolute first-law residual remains below 0.9% on all four schedules. The full schedules are enforced by `regulatory_cycle_tracking_regression`; US06 is not reclassified by weakening its tolerance band.

### First-law physics ledger

```text
physics status|ledger|report
physics reset
physics export <report.txt>
```

The ledger accumulates fuel chemical energy, indicated/brake work, heat rejection, friction, pumping, accessories, driveline/converter/tire/brake losses, road load, grade work, and kinetic-energy change without forcing the residual to zero.

### Automated calibration and uncertainty

```text
calibrate vehicle fit [observations.csv] [iterations]
calibrate vehicle status|apply|restore
uncertainty vehicle run [samples] [seed]
uncertainty vehicle status
```

Calibration is bounded, uncertainty-weighted, transactional, and idempotent on repeated apply. Uncertainty runs are deterministic for a fixed seed and report 90%/95% intervals plus sensitivity shares.

See `docs/MUZIXDIAGSYS_USER_MANUAL.md`, section **8.14**, for equations, CSV formats, safety limits, validation interpretation, and a complete coupled workflow.


## Advanced six-DOF vehicle realism

MuzixDiagSys includes an integrated six-degree-of-freedom body, four-corner sprung/unsprung suspension, combined-slip thermal tires, compliant driveline/differential, OpenDRIVE/OpenCRG/OpenSCENARIO execution, production-style ECU scheduling, shared XCP/A2L and MDF measurement access, multi-experiment Bayesian calibration, and progressive component degradation.

See [`docs/ADVANCED_VEHICLE_REALISM.md`](docs/ADVANCED_VEHICLE_REALISM.md) for exact commands, file formats, physical assumptions, and validation procedures.


## Perception, ODD, digital-twin, and measurement realism

The advanced vehicle platform now couples physical EPS/rack/Ackermann steering, suspension kinematics, five-dimensional aerodynamic maps, OpenMATERIAL-derived surface properties, delayed/noisy camera-radar-lidar-ultrasonic models, OSI/OSMP exchange, OpenODD scenario synthesis, sensor fusion/localization, bounded digital-twin estimation, brake/tire/road-dust particulate emissions, and virtual PEMS instrumentation into the existing six-DOF plant.

Exact command families:

```text
industrial vehicle steering|kinematics ...
industrial vehicle aero|aerodynamics ...
industrial vehicle material|openmaterial ...
industrial vehicle sensor|perception ...
industrial vehicle osmp ...
industrial vehicle odd|openodd ...
industrial vehicle fusion|localization ...
industrial vehicle twin|digital-twin ...
industrial vehicle nonexhaust|particulate ...
industrial vehicle pems ...
```

All measurements and writable calibrations use the existing industrial signal registry, XCP/A2L service, and MDF 4.10 recorder. See [`docs/ADVANCED_VEHICLE_REALISM.md`](docs/ADVANCED_VEHICLE_REALISM.md) for exact syntax, file formats, equations, limits, and a complete workflow. Example material data is supplied in `data/vehicle_openmaterial.json`.

## Full electrified-vehicle architecture

MuzixDiagSys now includes a concrete integrated BEV, series-hybrid, parallel-hybrid, plug-in-hybrid, and fuel-cell vehicle stack with an electrothermal battery/BMS, dual-machine e-axles, map-based motoring and regeneration, hydraulic brake-by-wire blending, active suspension/rear steering, trailer and load-shift dynamics, DOC/TWC/DPF/SCR chemistry, Automotive Ethernet/SOME-IP/TSN distributed ECUs, SOVD/OTA lifecycle, automated SOTIF falsification, regulatory durability accumulation, and online digital-twin assimilation.

```text
industrial energy advanced status
industrial energy advanced auto on|off
industrial energy advanced architecture bev|series|parallel|phev|fuel-cell
industrial energy advanced payload set <id> <kg> <x_m> <y_m> <z_m> <longitudinal_restraint_n> [lateral_restraint_n] [compliance_m_n]
industrial energy advanced sotif aeb [generations]
industrial energy advanced network|sovd|ota
```

See [`docs/ADVANCED_ELECTRIFIED_VEHICLE_IMPLEMENTATION.md`](docs/ADVANCED_ELECTRIFIED_VEHICLE_IMPLEMENTATION.md) for the implementation matrix, model equations, calibration-map format, API example, and verification coverage. These are engineering simulation and virtual-verification models, not an external standards or regulatory certification.


## High-fidelity multiphysics vehicle layer

The electrification runtime now also exposes a deterministic multi-rate vehicle layer that couples a conservative scheduler, compliant multibody suspension, flexible-ring tires, a torsional driveline, a distributed thermal graph, uncertain/faulted sensors, network-timed ECU execution, crank-angle combustion and one-dimensional gas paths, a cell-resolved electrochemical battery, and automated calibration/validation/uncertainty quantification.

```text
industrial energy high-fidelity status
industrial energy high-fidelity auto on|off
industrial energy high-fidelity reset [ambient_k]
industrial energy high-fidelity step [dt_s] [rpm torque_nm speed_m_s wheel_torque_nm brake]
industrial energy high-fidelity road <mu> <roughness_m> [water_m] [loose_m]
industrial energy high-fidelity steering <rad>
industrial energy high-fidelity sensor-fault <sensor> <mode> <id> <start_s> <duration_s> <magnitude> [secondary] [duty] [period_s]
industrial energy high-fidelity sensor-clear
industrial energy high-fidelity battery-short <series> <parallel> <resistance_ohm>
industrial energy high-fidelity calibrate [iterations] [folds] [uq_samples]
industrial energy high-fidelity assurance-export <output.json>
industrial energy high-fidelity solver|suspension|tires|driveline|thermal|sensors|ecu|engine|battery
```

See [`docs/HIGH_FIDELITY_MULTIPHYSICS_IMPLEMENTATION.md`](docs/HIGH_FIDELITY_MULTIPHYSICS_IMPLEMENTATION.md) for model equations, execution rates, fault modes, signal names, C++ integration, and validation coverage.


## Next-generation vehicle-depth runtime (2026-07-12)

The additive `industrial energy depth` runtime couples flexible-body modal dynamics, three-dimensional environmental terrain, advanced structural tires, distributed HV protection transients, switching-resolved electric drive behavior, multidimensional aero-thermal flow, detailed brake hydraulics and tribology, AUTOSAR-oriented multicore scheduling, deterministic checkpoint/branch replay, and state-conserving multi-fidelity transitions.

```text
industrial energy depth status
industrial energy depth step 0.02 2200 140 20 900 0.10
industrial energy depth checkpoint baseline
industrial energy depth branch lower-demand baseline
industrial energy depth branch-select lower-demand
industrial energy depth counterfactual 0 wheel_torque_nm 250 reduced-demand
industrial energy depth replay
industrial energy depth fidelity tire detailed
industrial energy depth structure
industrial energy depth terrain
industrial energy depth tires
industrial energy depth hv
industrial energy depth drive
industrial energy depth aero
industrial energy depth brakes
industrial energy depth autosar
```

The complete implementation and operator reference is [`docs/NEXT_GENERATION_VEHICLE_DEPTH_IMPLEMENTATION.md`](docs/NEXT_GENERATION_VEHICLE_DEPTH_IMPLEMENTATION.md). Validation criteria are in [`docs/NEXT_GENERATION_VEHICLE_DEPTH_VALIDATION.md`](docs/NEXT_GENERATION_VEHICLE_DEPTH_VALIDATION.md), and the comprehensive manual is [`docs/MUZIXDIAGSYS_USER_MANUAL.md`](docs/MUZIXDIAGSYS_USER_MANUAL.md).

## Integrated vehicle–occupant–environment ecosystem (2026-07-12)

The additive `industrial energy ecosystem` runtime couples the complete next-generation vehicle-depth model to a conservative thermo-fluid network, cranktrain/valvetrain/EHL bearings, injection and spray combustion, full transmission internals, particle-scale battery aging and propagation, raw radar/camera/lidar signals, human takeover behavior, interactive traffic/V2X/formal ODD, mechanism-based durability/RUL, and FMI/OpenX Offline/SIL/PIL/HIL execution.

```text
industrial energy ecosystem status
industrial energy ecosystem step 0.02 2200 150 20 900 0.05 24
industrial energy ecosystem driver-mode automated
industrial energy ecosystem execution-mode sil off
industrial energy ecosystem traffic-add lead-01 car 60 0 18 24 on
industrial energy ecosystem signal-add junction-a 250 30 35 4 0
industrial energy ecosystem environment 8 450 0.05 4000
industrial energy ecosystem odd-set 253.15 323.15 35 80 0.12 0.35 36 on off off
industrial energy ecosystem battery-short 17 0.03
industrial energy ecosystem battery-short-clear 17
industrial energy ecosystem export ./ecosystem_openx
industrial energy ecosystem thermofluid
industrial energy ecosystem cranktrain
industrial energy ecosystem combustion
industrial energy ecosystem transmission
industrial energy ecosystem particle-battery
industrial energy ecosystem sensors
industrial energy ecosystem driver
industrial energy ecosystem traffic
industrial energy ecosystem durability
industrial energy ecosystem realtime
industrial energy ecosystem interop
```

The public C++ facade is `aesim::high_fidelity::IntegratedVehicleEcosystemRuntime` in `include/aesim/high_fidelity/ecosystem.hpp`. Detailed equations, coupling, commands, signals, calibration, and validation are documented in [`docs/VEHICLE_ECOSYSTEM_IMPLEMENTATION.md`](docs/VEHICLE_ECOSYSTEM_IMPLEMENTATION.md), [`docs/VEHICLE_ECOSYSTEM_VALIDATION.md`](docs/VEHICLE_ECOSYSTEM_VALIDATION.md), and the updated [`docs/MUZIXDIAGSYS_USER_MANUAL.md`](docs/MUZIXDIAGSYS_USER_MANUAL.md).


## Full lifecycle virtual vehicle: crash, fire, CFD, NVH, degradation and autonomy

The additive `industrial energy lifecycle` runtime extends the complete ecosystem with nonlinear crash and occupant restraints, battery vent-gas/fire/enclosure pressure, reduced-order three-dimensional CFD/CHT, unified tribology/wear, structural acoustics and psychoacoustics, power-electronics lifetime, environmental ingress/corrosion/icing, steering road feel, predictive energy/thermal/chassis control, and a complete autonomous perception-prediction-planning-control chain.

```text
industrial energy lifecycle status
industrial energy lifecycle step 0.04 1800 100 12 650 0.02 18
industrial energy lifecycle autonomy-mode active
industrial energy lifecycle crash front 8.0 0.8
industrial energy lifecycle battery-fire 0 5000
industrial energy lifecycle weather 10 268.15 3.0 0.02 0.85
industrial energy lifecycle cfd
industrial energy lifecycle tribology
industrial energy lifecycle nvh
industrial energy lifecycle power-electronics
industrial energy lifecycle exposure
industrial energy lifecycle steering
```

See `docs/FULL_LIFECYCLE_VIRTUAL_VEHICLE_IMPLEMENTATION.md` and `docs/FULL_LIFECYCLE_VIRTUAL_VEHICLE_VALIDATION.md`.

## Software-only simulation experience platform (2026-07-12)

The additive `industrial experience` runtime provides persistent vehicle ownership and service history, deterministic scenario timelines and branches, causal explanations, physics-driven WAV audio, OpenCRG/procedural road surfaces, distributed tire contact, suspension compliance, dynamic weather and road state, heterogeneous traffic, diagnostic workshop cases, ASCII/SVG visualization, reference-ghost comparison, adaptive fidelity, uncertainty reports, and a live human driver skill model. No dedicated simulation hardware is required.

```text
industrial experience garage create commuter_01 compact_sedan turbo_i4
industrial experience timeline load data/experience/urban_wet_timeline.yaml
industrial experience road generate worn_city 42 5000 10 0.008 7 0.012 0.90 asphalt
industrial experience weather add storm 0 0 1200 4 0 35 0 300 12 3 286
industrial experience traffic populate 80 5000 91422
industrial experience driver transmission manual 6
industrial experience driver target 25
industrial experience driver on
industrial experience audio start 60
industrial experience visual load-ghost data/experience/reference_ghost.csv
industrial experience report automatic markdown ./experience_report.md
```

See [`docs/SOFTWARE_SIMULATION_EXPERIENCE_PLATFORM.md`](docs/SOFTWARE_SIMULATION_EXPERIENCE_PLATFORM.md) for architecture, equations and state coupling, all commands, sample workflows, and validation coverage.

## Virtual automotive laboratory

The software-only laboratory adds component-level vehicle construction, compatibility validation, tuning, engine/chassis/transmission/battery benches, deterministic engineering recommendations, telemetry replay, crash reconstruction, procedural worlds and missions, manufacturing variation, teardown analysis, and an ABI-v2 modding SDK.

```text
industrial vehicle experience lab status
industrial vehicle experience lab builder catalog data/lab/component_catalog.yaml
industrial vehicle experience lab builder new track_car
industrial vehicle experience lab dyno engine 1000 7000 250
industrial vehicle experience lab engineer investigate cold shift flare
```

See `docs/VIRTUAL_AUTOMOTIVE_LAB_PLATFORM.md` and `docs/sdk/MUZIXDIAGSYS_MODDING_SDK.md`.

## Guarded CAN, OBD-II, and automotive data synthesis

The virtual automotive laboratory now includes a guarded CAN/OBD gateway with Linux SocketCAN and loopback backends, functional OBD-II services, ISO-TP response assembly, capture/import/export, trace intelligence, and deterministic labelled multi-ECU CAN/CAN-FD synthesis. Real-interface transmission is disabled by default and requires explicit diagnostic or raw allow-list access.

Primary commands:

```text
industrial vehicle experience lab can ...
industrial vehicle experience lab obd ...
industrial vehicle experience lab synthesis ...
```

See `docs/CAN_OBD_DATA_SYNTHESIS_PLATFORM.md` and `data/lab/can_obd_demo_commands.txt` for the safety model, live-adapter setup, supported PIDs/services, trace analytics, generated cycles/faults, counterfactual augmentation, and export formats.

## SocketCAN OBD-II vehicle responder

MuzixDiagSys can operate as a vehicle-side OBD-II ECU on an isolated Linux SocketCAN bench bus. It accepts functional and physical ISO-TP requests, publishes live simulated PIDs, exposes confirmed/pending/permanent DTCs and freeze frames, and supports multi-frame VIN and diagnostic responses.

See [`docs/SOCKETCAN_OBD_RESPONDER.md`](docs/SOCKETCAN_OBD_RESPONDER.md) and [`data/lab/obd_responder_demo_commands.txt`](data/lab/obd_responder_demo_commands.txt).

## Lean source tree and reproducible packaging

MuzixDiagSys keeps generated study output, exported FMUs/DBCs, generated command
documentation, and local build products out of the authoritative source tree.
This avoids shipping stale results and prevents a compatibility launcher from
doubling the build footprint.

Create a deterministic source-only archive:

```bash
cmake --build build --target source_package
# or directly:
python3 tools/package_source.py MuzixDiagSys-source.zip
```

Remove only reproducible local output:

```bash
cmake --build build --target clean_generated_artifacts
```

On Unix developer builds, `engine_sim` is a symbolic link to the primary
`muzixdiagsys` executable, eliminating a second full binary image. Mutable
`data`, `plugins`, and `configs` remain isolated build-local copies so tests and
runtime exports cannot modify the source checkout. Installed packages contain
ordinary files and directories.

## Integrated Engineering Studio

The canonical `studio` command opens the cross-domain engineering workbench. It provides a unified typed action/service layer, live signal explorer, synchronized timeline, schema-generated forms, time-travel debugger, executable contracts, differential validation, scenario minimization, reproducible bug capsules, calibration-map editing, co-simulation topology management, solver/performance analysis, confidence-aware results, and virtual manufacturing/EOL campaigns.

```text
studio status
studio action list
studio signals list engine
studio debug checkpoint baseline
studio contracts evaluate
studio topology validate
studio performance recommend
studio manufacturing demo 100 reports/eol-lot 42
```

See [`docs/ENGINEERING_STUDIO.md`](docs/ENGINEERING_STUDIO.md) for the complete command, architecture, artifact, and validation reference.

## Causal simulation, resilience, and differentiable analysis laboratory

MuzixDiagSys now includes an integrated C++17 causal simulation
laboratory providing deterministic time-travel debugging, graph-aware run
difference analysis, structured observability, Bayesian causal diagnostics,
real-world scenario mining, multi-modal sensor simulation, cyber-physical attack
campaigns, graceful-degradation analysis, rare-event acceleration, and
forward/adjoint differentiable simulation.

Public API:

```cpp
#include "aesim/research2/causal_simulation.hpp"
```

Build and inspect the command-line utility:

```bash
cmake -S . -B build -DAESIM_BUILD_TESTS=ON -DAESIM_BUILD_TOOLS=ON
cmake --build build -j
./build/muzixdiagsys_causal_lab status
ctest --test-dir build -R causal_simulation_unit_tests --output-on-failure
```

Operational commands include timeline hash verification, deterministic run
comparison, CSV scenario mining, and a Gaussian rare-event reference analysis.
See [`docs/CAUSAL_SIMULATION_LAB.md`](docs/CAUSAL_SIMULATION_LAB.md) and
[`CAUSAL_SIMULATION_IMPLEMENTATION_REPORT_2026-07-15.md`](CAUSAL_SIMULATION_IMPLEMENTATION_REPORT_2026-07-15.md).

## Specification, Discovery, and Verification Suite

MuzixDiagSys includes an integrated specification/discovery layer for temporal requirements, counterexample minimization, MAP-Elites scenario exploration, property and mutation testing, formal verification, compositional contracts, safety-shield synthesis, Bayesian experiment planning, causal-path coverage, raw sensor rendering, Byzantine-resilient cooperative perception, cyberattack optimization, forensic reconstruction, hierarchical fleet twins, and change-point detection.

```bash
./build/muzixdiagsys_specification_discovery capabilities
./build/muzixdiagsys_specification_discovery self-test
./build/muzixdiagsys_specification_discovery synthesize-monitor \
  'response brake > 0.5 -> eventually[0,0.25] decel < -2.0'
```

See `docs/SPECIFICATION_DISCOVERY_VERIFICATION_SUITE.md` for the API and algorithm reference.

## Advanced cyber-physical platform

MuzixDiagSys now includes an additive advanced-platform library and CLI covering native ROS 2/rosbag2, CARLA, Autoware, Apollo, Gymnasium/PettingZoo, multi-objective optimization, HARA/FMEA/FMEDA/FTA/STPA, stateful automotive protocol fuzzing, HSM/secure boot/SecOC/OTA/attestation, digital homologation, Arrow/Parquet storage, Slurm/Kubernetes execution, and deterministic CPU/GPU graphs.

Build target and executable:

```bash
cmake --build build --target muzixdiagsys_advanced_platform advanced_platform_tests
build/muzixdiagsys_advanced_platform self-test build/advanced-platform-self-test
```

Complete schemas, examples, security behavior, and command usage are documented in [`docs/ADVANCED_CYBER_PHYSICAL_PLATFORM.md`](docs/ADVANCED_CYBER_PHYSICAL_PLATFORM.md). Ready-to-run inputs are under [`examples/advanced_platform/`](examples/advanced_platform/).

## Next-generation automotive research and deployment platform

The advanced library now also includes a typed simulation compiler with MLIR emission, formal controller and safety-architecture synthesis, graph-level ONNX verification, a COVESA/Eclipse-style SDV runtime, real OpenSSL 3.5 post-quantum cryptography, HSM attack campaigns, NR-V2X/NTN/edge co-simulation, OpenUSD synthetic datasets, rare-event reliability methods, cycle-accurate ECU/NPU timing, embedded C generation with MIL/SIL/PIL/HIL equivalence, manufacturing/EOL simulation, and fleet prognostics with robust federated aggregation.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release -DBUILD_TESTING=ON
cmake --build build --target next_generation_platform_tests \
  muzixdiagsys_advanced_platform -j
./build/next_generation_platform_tests
./build/muzixdiagsys_advanced_platform self-test \
  build/next-generation-self-test build/next-generation-self-test.json
```

See [`docs/NEXT_GENERATION_AUTOMOTIVE_PLATFORM.md`](docs/NEXT_GENERATION_AUTOMOTIVE_PLATFORM.md) for the complete architecture, API, algorithms, and qualification reference. The executable reference workflow is in [`tests/next_generation_platform_tests.cpp`](tests/next_generation_platform_tests.cpp).

## Systems and lifecycle engineering platform

The advanced library now also includes SysML v2 digital-thread baselines and impact analysis, automated ARX identification and bounded nonlinear calibration, transient SPICE/EMC/wiring-harness co-simulation, cell-resolved battery abuse and thermal-runaway propagation, exact E/E architecture synthesis, conservative and optimistic distributed shared-world execution, physically based spectral dataset generation, dynamic city infrastructure simulation, occupant-restraint crash biomechanics, and mass-balanced lifecycle/circular-economy analysis.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release -DBUILD_TESTING=ON
cmake --build build --target digital_thread_lifecycle_tests \
  muzixdiagsys_advanced_platform -j
./build/digital_thread_lifecycle_tests
./build/muzixdiagsys_advanced_platform self-test \
  build/systems-lifecycle-self-test build/systems-lifecycle-self-test.json
```

See [`docs/SYSTEMS_LIFECYCLE_ENGINEERING_PLATFORM.md`](docs/SYSTEMS_LIFECYCLE_ENGINEERING_PLATFORM.md) for the full API, algorithms, evidence model, and qualification reference. A SysML v2 reference model and usage guide are available under [`examples/systems_lifecycle_platform/`](examples/systems_lifecycle_platform/).

## Continuous engineering, physical assurance, and service platform

The additive continuous-engineering extension connects executable scenario
coverage, localization integrity, AI lifecycle governance, robotic laboratory
execution, reduced-order multiphysics, tire and particle-emission physics,
fleet cyber operations, heterogeneous SoC synthesis, signed product passports,
and autonomous service planning.

Public API:

```cpp
#include "aesim/advanced/platform.hpp"
```

Build and run the dedicated qualification suite:

```bash
cmake -S . -B build -G Ninja \
  -DAESIM_BUILD_TESTS=ON \
  -DAESIM_BUILD_TOOLS=ON
cmake --build build --target \
  continuous_engineering_platform_tests \
  advanced_platform_cli
ctest --test-dir build \
  -R 'continuous_engineering_platform|advanced_platform_cli_self_test' \
  --output-on-failure
```

A typed scenario example is provided at
`examples/continuous_engineering_platform/emergency_braking.osc2`. See
[`docs/CONTINUOUS_ENGINEERING_PLATFORM.md`](docs/CONTINUOUS_ENGINEERING_PLATFORM.md)
for the complete architecture, algorithms, API behavior, numerical methods,
external-system boundaries, and qualification workflow.

## Qualification, trusted evidence, real-time deployment, and collaborative studio

The advanced platform now includes a unified compliance-evidence engine, qualified-tool and trusted-computation manifests, deterministic MDF/A2L/XCP measurement workflows, time-travel debugging, evidence-aware regression intelligence, fixed-priority/EDF timing qualification, AUTOSAR semantic round trips and code generation, end-to-end ADS metrics, CAD/mesh processing, and a governed collaborative engineering backend with a generated static web client.

```bash
cmake -S . -B build -DAESIM_BUILD_TESTS=ON -DAESIM_BUILD_TOOLS=ON
cmake --build build --target qualification_studio_platform_tests \
  muzixdiagsys_advanced_platform -j
ctest --test-dir build \
  -R 'qualification_studio_platform|advanced_platform_cli_self_test' \
  --output-on-failure
```

See [`docs/QUALIFICATION_COLLABORATIVE_ENGINEERING_PLATFORM.md`](docs/QUALIFICATION_COLLABORATIVE_ENGINEERING_PLATFORM.md) and [`examples/qualification_studio_platform/`](examples/qualification_studio_platform/) for the architecture, API behavior, external-system boundaries, and executable inputs.

## Next-generation engineering laboratories

The public header `include/aesim/advanced/next_generation_labs.hpp` provides five integrated engineering laboratories:

- `GeneralMultibodyWorld` for three-dimensional rigid-body, joint, friction, and contact dynamics.
- `RawSensorMetrologyLaboratory` for camera/radar/lidar calibration, uncertainty budgets, and Gauge R&R.
- `ContinuousAdsQualificationEngine` for field-event scenario extraction, ODD drift, cohort rates, and safety-case deltas.
- `InstructionAccurateRiscVSoC` for executable RV32I/RV32M virtual ECU and memory-mapped peripheral simulation.
- `DifferentiableVehicleControllerCoDesigner` for robust mixed discrete/continuous constrained co-design.

See `NEXT_GENERATION_LABS_IMPLEMENTATION_REPORT_2026-07-16.md` and the `next_generation_labs_tests` target for executable examples and verification coverage.


## Formula One Frontier Laboratory

The advanced Formula One stack now also includes a minimum-lap-time racing-line and control solver; unsteady moving-ground CFD with rotating-wheel wakes and aeroelastic FSI; ATR/cost-cap development portfolio optimization; composite survival-cell crash homologation; serialized tyre-set weekend allocation; qualifying release, traffic, and tow optimization; formation-lap and grid-start launch simulation; high-rate DAQ and telemetry bandwidth architecture; predictive neutralization risk; and causal microsector driver coaching. See `docs/FORMULA_ONE_FRONTIER_LABORATORY.md`.

## Formula One engineering platform

The advanced library includes a Formula One-specific engineering layer with:

- versioned 2026 FIA Section C compliance profiles and rule-delta analysis;
- a 2026 hybrid power-unit and lap energy-management laboratory;
- active front/rear aerodynamics, ground effect, aeroelasticity, and porpoising;
- tire pressure, thermal state, degradation, wet performance, and track evolution;
- race-strategy optimization, Monte Carlo race analysis, and pit-wall decisions.

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build --target formula_one_platform_tests -j
ctest --test-dir build -R formula_one_platform_unit_tests --output-on-failure
```

See [`docs/FORMULA_ONE_PLATFORM.md`](docs/FORMULA_ONE_PLATFORM.md) for the complete
API, numerical behavior, validation workflow, and qualification boundaries.

## Formula One race-engineering digital twin

The additive Formula One race-engineering module provides:

- coupled suspension heave, pitch, roll, steering, wheel-hop, anti-roll, third-element, bump-stop, plank-contact, and setup optimization;
- carbon brake, brake-by-wire, regenerative blending, wheel-end thermal, wear, lockup, and hydraulic-fallback physics;
- survey-derived circuit cells with spatial weather, track evolution, contamination, water film, grip, and aerodynamic wake effects;
- ensemble telemetry assimilation, anomaly detection, hidden-state estimation, and live pit-wall advice;
- Weibull/thermal/shock component lifing, damage events, and championship-weighted component allocation.

Build and run the dedicated validation target:

```bash
cmake --build build --target formula_one_race_engineering_tests -j
ctest --test-dir build -R formula_one_race_engineering_unit_tests --output-on-failure
```

See `docs/FORMULA_ONE_RACE_ENGINEERING.md` for the API and workflow guide.

## Silicon, Human, Infrastructure, and Heterogeneous Execution Platform

The advanced platform now exports production laboratories for heterogeneous ECU/SoC timing and thermal behavior, formally synthesized fault-tolerant control, device-level camera/lidar/radar rendering with pose derivatives, digital-human injury and cognitive response, crash and post-crash consequences, V2G infrastructure dispatch, non-exhaust particle emissions, lifecycle circularity, hardware side-channel analysis, and heterogeneous kernel compilation with reverse-mode gradients.

Use the public C++ API through:

```cpp
#include "aesim/advanced/silicon_human_infrastructure_platform.hpp"
```

See `docs/silicon_human_infrastructure_platform.md` for model contracts and result semantics.

## Atomistic, Device, Infrastructure, and Remote-Operations Platform

The advanced library now includes production implementations for atomistic molecular dynamics and tight-binding quantum materials, 1D semiconductor TCAD and reliability, adaptive conservative PDE/mesh execution, explicit 3D crash and human injury mechanics, fire/smoke/suppression, coupled vibroacoustics and aeroacoustics, pavement/bridge infrastructure twins, CT and ultrasonic NDE, RTL-to-binary co-verification, and remote-assistance/teleoperation operations.

```cpp
#include "aesim/advanced/atomistic_remote_operations_platform.hpp"
```

See `docs/atomistic_remote_operations_platform.md` for numerical contracts and result semantics.

## Architecture, Intelligence, and Sustainability Platform

The advanced platform now includes production implementations for architecture-level multidisciplinary design optimization, sparse physical-law discovery, PDE-constrained data assimilation, electronics packaging/PCB/harness reliability, complex wave optics and metasurface optimization, cabin microclimate and human thermoregulation, fuel-cell/electrolyzer/synthetic-fuel systems, smart-material morphing structures, autonomous maintenance/remanufacturing, and process-level recycling physics.

Public API:

```cpp
#include "aesim/advanced/architecture_intelligence_sustainability_platform.hpp"
```

Engineering reference: `docs/ARCHITECTURE_INTELLIGENCE_SUSTAINABILITY_PLATFORM.md`.


## Next-Generation Autonomy, Security, Energy, and Fabrication Platform

The advanced platform now provides production laboratories for multimodal driving world models,
cooperative V2X perception and edge scheduling, event-driven neuromorphic sensing, post-quantum
migration and confidential-compute qualification, beyond-lithium battery chemistry, resilient
PNT and quantum-sensor integration, extreme-weather resilience, differentiable generative CAD,
autonomous engineering evidence workflows, and semiconductor fabrication/yield simulation.

```cpp
#include "aesim/advanced/next_generation_autonomy_platform.hpp"
```

Engineering and numerical reference: `docs/NEXT_GENERATION_AUTONOMY_PLATFORM.md`.

## Frontier compute, energy, robotics, proof, and risk platform

The advanced platform now includes production C++ laboratories for 3D-IC/UCIe chiplet physical design, analog compute-in-memory and photonic acceleration, dynamic wireless charging, plasma and arc faults, quantum/tensor-network simulation, hybrid storage, embodied manipulation, agent-based mobility markets, proof-carrying numerical execution, and warranty/reliability economics. See `docs/FRONTIER_COMPUTE_ENERGY_RISK_PLATFORM.md`.


## Certified Deployment and Infrastructure Platform (2026-07-19)

The advanced library now includes ten production-oriented laboratories in `aesim/advanced/certified_deployment_infrastructure_platform.hpp`: a domain-bounded ridge neural-operator/surrogate compiler with generated C++ export and evidence hashing; an end-to-end differentiable linear co-simulation runtime; AI calibration, abstention and OOD assessment; switching/thermal EMT power-electronics analysis; conservative multiphase thermal-fluid/slosh simulation; functional-safety SoC fault injection and ISO 26262-style metrics; Bayesian accident reconstruction; Ed25519 signed evidence and verification; fleet shadow/canary guardrails; and radial charging-grid voltage, loss, thermal and protection assessment. All APIs reject malformed or non-finite configurations and are covered by native unit tests.


## Assured Engineering Operations Platform (2026-07-19)

The advanced library now exposes a unified implementation of ten additional
engineering systems through:

```cpp
#include "aesim/advanced/assured_engineering_operations_platform.hpp"
```

The platform includes:

- contract-driven co-simulation compilation with unit, frame, causality,
  rate-transition, algebraic-loop, rollback, and conservation qualification;
- certified linear-Gaussian filtering, Rauch--Tung--Striebel smoothing,
  multi-chain Metropolis sampling, credible intervals, effective sample size,
  and convergence diagnostics;
- scenario-based distributionally robust control with expected, worst-case,
  CVaR, chance-constraint, and Wasserstein ambiguity objectives;
- deterministic automotive controller synthesis, bounded generated C,
  requirement traceability, WCET/stack estimates, discharged proof
  obligations, SHA-256 binding, and Ed25519 evidence;
- crystal-slip integration, irreversible phase-field fracture, joint strength
  and fatigue qualification, and transient gigacasting solidification;
- dependency-aware robotic test-cell scheduling, capability and power
  matching, path/exclusion-zone checks, calibration/interlock enforcement,
  deterministic measurement-quality retries, and audit evidence;
- post-crash thermal growth, toxic-species generation/removal, road-network
  responder routing, protected responder dose, extraction timing, and occupant
  survival estimation;
- megawatt/depot charging dispatch with charger thermal derating, transformer
  limits, onsite storage, battery swapping, tariffs, carbon, demand charges,
  degradation, and departure readiness;
- policy-enforced differentially private engineering aggregation and a genuine
  P-256 Fiat--Shamir Schnorr zero-knowledge proof of secret knowledge; and
- propensity-score causal estimation, inverse-probability weighting,
  treatment-effect uncertainty, Crow--AMSAA reliability growth, and ranked
  candidate root causes.

Build and execute the dedicated regression target:

```bash
cmake -S . -B build -G Ninja -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build --target assured_engineering_operations_platform_tests -j
ctest --test-dir build \
  -R assured_engineering_operations_platform_unit_tests \
  --output-on-failure
```

Detailed model contracts, algorithms, numerical limitations, and qualification
semantics are documented in
[`docs/ASSURED_ENGINEERING_OPERATIONS_PLATFORM.md`](docs/ASSURED_ENGINEERING_OPERATIONS_PLATFORM.md).

## Operational Digital Infrastructure Platform

The advanced library now includes a live semantic telemetry fabric, bounded formal source/binary/RTL refinement, nonlinear electromagnetic-machine finite elements, fleet OTA compatibility and rollback qualification, a mixed-criticality SDV service mesh, space-weather and single-event reliability, a neuromusculoskeletal digital human, hydrogen materials and cryogenic-transfer safety, 6G integrated sensing/communications, and cascading multi-infrastructure disaster restoration. See `docs/OPERATIONAL_DIGITAL_INFRASTRUCTURE_PLATFORM.md`.

## Formula One Physical Operations Laboratory

The advanced library now includes a Formula One physical-and-operations platform covering fuel and dry-sump mass migration, layered tyre/contact-patch physics, shared hydraulic actuation, laser-scanned track contact, parc-ferme provenance, season component/logistics optimization, composite manufacture/NDT/repair, trackside weather nowcasting, pit-wall human decision simulation, and wheel-corner/wheel-nut qualification. See `docs/FORMULA_ONE_PHYSICAL_OPERATIONS_LABORATORY.md`.

## IndyCar IR-18 Engineering and Competition Platform

The advanced library now includes a versioned IndyCar IR-18 rules and vehicle platform; banked oval, short-oval, and superspeedway dynamics; pack-racing wake and side-draft analysis; driver-only weight-jacker and roll-bar control; hybrid regeneration, self-start, and push-to-pass orchestration; serialized Firestone tyre strategy without warmers; Indianapolis 500 preparation; road/street and oval qualifying; race-control and pit-lane state transitions; and sealed engine/hybrid pool lifing. See `docs/INDYCAR_PLATFORM.md`.


## IndyCar Operations, Compliance, and Human Performance Platform

The advanced library includes ten additional IndyCar laboratories through:

```cpp
#include "aesim/advanced/indycar_operations_platform.hpp"
```

The module provides regulated event fuel allotments and gravity refueling,
resolved renewable-ethanol twin-turbo V6 thermodynamics and durability,
aeroscreen optics/cooling/impact analysis, deterministic spotter and radio
reliability, guard-banded technical inspection, locked calibration and mandatory
telemetry verification, legal test/ROP/refresher allocation, primary/backup car
crash recovery, seven-person pit-crew and wheel-gun simulation, and transient
street-circuit bump/brake/wall loading. See
[`docs/INDYCAR_OPERATIONS_PLATFORM.md`](docs/INDYCAR_OPERATIONS_PLATFORM.md).

Build and execute the dedicated regression with:

```bash
cmake -S . -B build -G Ninja -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build --target indycar_operations_platform_tests -j
ctest --test-dir build -R indycar_operations_platform_unit_tests --output-on-failure
```

## Automotive Standards and Conformance Platform

The advanced platform now includes executable models for ASAM Quality/QSQ, ASAM CEA, ASAM OpenTestSpecification, UN R171 DCAS, ISO/SAE 21434 with UN R155/R156 and ISO 24089, ISO 26262-11 semiconductor safety, SAE J3400 with ISO 15118-20, CAN XL, 10BASE-T1S/PLCA, automotive SerDes, and CCC Digital Key.

See [`docs/AUTOMOTIVE_STANDARDS_CONFORMANCE_PLATFORM.md`](docs/AUTOMOTIVE_STANDARDS_CONFORMANCE_PLATFORM.md) and [`examples/automotive_standards/`](examples/automotive_standards/).


## Emerging mobility platform

Ten new laboratories cover 3D Gaussian Splatting, AAOS cockpit, AR-HUD, cabin sensing, SAE J2601, multi-gig Ethernet, Release 18 V2X, SOAFEE/WASM, FPGA-HIL, and UN R157/R160/DSSAD. See `docs/EMERGING_MOBILITY_PLATFORM.md`.

## Formula One Championship Operations Platform

The advanced library now includes official timing and classification, trackside safety and restart readiness, cost-cap forensics, fuel and oil chemical certification, F1 ERS high-voltage safety, driver-cooling Heat-Hazard qualification, wet-weather spray visibility, active-aero actuator fail-safe qualification, physical anti-circumvention scrutineering, and calibrated-camera sporting evidence. See [`docs/FORMULA_ONE_CHAMPIONSHIP_OPERATIONS.md`](docs/FORMULA_ONE_CHAMPIONSHIP_OPERATIONS.md) and [`examples/formula_one_championship_operations/`](examples/formula_one_championship_operations/).

## NASCAR Competition Platform

The advanced executable now includes a dedicated `nascar` command family for
Cup Next Gen dynamics, superspeedway pack racing, NASCAR race control, the 2026
Chase and stage championship, timing/SMT, single-lug pit crews, Goodyear tyre
and wet-weather behavior, evolving track surfaces, OSS inspection, and Next Gen
crash/roof-flap/SAFER-barrier safety.

```bash
./build/full/muzixdiagsys_advanced_platform nascar capabilities
./build/full/muzixdiagsys_advanced_platform nascar self-test \
  build/full/nascar-self-test build/full/nascar-self-test.json
```

See `docs/NASCAR_COMPETITION_PLATFORM.md` and
`examples/nascar_competition/`.

## Formula One regulatory and competition platform (2026-07-23)

The additive Formula One platform is exported through
`include/aesim/advanced/formula_one_regulatory_competition_platform.hpp`,
compiled into `aesim_formula_one`, and available transitively from
`aesim_advanced`. It does not alter the existing IndyCar or NASCAR public
platforms.

The `f1-regulatory` CLI family exposes ten production domains:

```text
ers-electrical-hardware
full-field-competition
championship-governance
power-unit-governance
operational-restrictions
remote-race-control
pit-lane-vision
regulatory-case-law
accident-reconstruction
circuit-homologation
```

Public entry points are `F12026ErsElectrothermalLaboratory`,
`F1FullFieldCompetitionEngine`, `F1ChampionshipGovernancePlatform`,
`F1PowerUnitHomologationPlatform`, `F1OperationalRestrictionsPlatform`,
`F1RemoteRaceControlFusionCenter`, `F1PitLaneVisionOfficiatingPlatform`,
`F1RegulatoryCaseLawCompiler`, `F1AccidentReconstructionLaboratory`, and
`F1CircuitHomologationPlatform`.

```bash
cmake -S . -B build/f1-regulatory -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON
cmake --build build/f1-regulatory --parallel --target \
  aesim_formula_one muzixdiagsys_advanced_platform \
  formula_one_regulatory_competition_platform_tests
ctest --test-dir build/f1-regulatory --output-on-failure \
  -R '^formula_one_.*_unit_tests$'
./build/f1-regulatory/muzixdiagsys_advanced_platform \
  f1-regulatory self-test build/f1-evidence build/f1-self-test.json
```

Canonical requests are in `examples/formula_one_regulatory_competition/`.
The complete API, input contracts, output semantics, qualification boundaries,
and validation sequence are documented in
`docs/FORMULA_ONE_REGULATORY_COMPETITION_PLATFORM.md`.

## Formula One industrial and ecosystem platform (2026-07-24)

The Formula One-only industrial expansion is exported through
`include/aesim/advanced/formula_one_industrial_ecosystem_platform.hpp` and
compiled into the focused `aesim_formula_one_industrial` library. The focused
library is linked publicly into `aesim_formula_one`, preserving all existing
Formula One, IndyCar, and NASCAR features while avoiding cross-series source
changes.

The `f1-industrial` CLI family provides ten domains for PU manufacturer
financial compliance, Pirelli production and metrology, sustainable-fuel
production, factory manufacture, vehicle assembly variation, causal setup
intelligence, aerodynamic raceability design, cyber/RF resilience, driver
medical performance, and the F2/F3/F1 Academy ladder.

```bash
cmake -S . -B build/f1-industrial -G Ninja \
  -DCMAKE_BUILD_TYPE=RelWithDebInfo -DBUILD_TESTING=ON
cmake --build build/f1-industrial --parallel --target \
  aesim_formula_one_industrial \
  formula_one_industrial_ecosystem_platform_tests
ctest --test-dir build/f1-industrial --output-on-failure \
  -R '^formula_one_industrial_ecosystem_platform_unit_tests$'
```

See [`docs/FORMULA_ONE_INDUSTRIAL_ECOSYSTEM_PLATFORM.md`](docs/FORMULA_ONE_INDUSTRIAL_ECOSYSTEM_PLATFORM.md)
and [`examples/formula_one_industrial_ecosystem/`](examples/formula_one_industrial_ecosystem/).

## Generalized scientific simulation platform (2026-07-26)

The additive generalized platform is exported through
`include/aesim/advanced/generalized_simulation_platform.hpp` and compiled into
`aesim_advanced`. It preserves every existing simulator feature while adding
shared services for deterministic distributed task execution, coordinated
content-addressed checkpoint/restart, unified mesh and field operations,
hardware-aware solver selection, high-index DAE compilation, cross-solver
verification, executable benchmark registration, SQL scientific analytics,
HTTP/notebook control, and cross-platform deterministic-equivalence testing.

```bash
cmake -S . -B build/generalized -G Ninja \
  -DCMAKE_BUILD_TYPE=Debug -DBUILD_TESTING=ON \
  -DAESIM_MAX_PARALLEL_COMPILES=2
cmake --build build/generalized --parallel 2 --target \
  generalized_simulation_platform_tests
ctest --test-dir build/generalized --output-on-failure \
  -R '^generalized_simulation_platform_(unit_tests|source_regression)$'
```

See [`docs/GENERALIZED_SIMULATION_PLATFORM.md`](docs/GENERALIZED_SIMULATION_PLATFORM.md)
and Chapter 51 of the comprehensive user manual.


## Formula One integrated realism platform

The current source includes `formula_one_realism_platform.hpp`, providing hardpoint suspension K&C, flexible-ring tyres, circuit microclimate/drainage/debris/spray, damage-aware performance, human driver dynamics, wheel-end/driveline mechanics, trackside RF/EMC, tyre pedigree inference, counterfactual race engineering, and wind-tunnel facility metrology. See `docs/FORMULA_ONE_REALISM_PLATFORM.md` and Chapter 53 of the user manual.


## Continuum Reality, Multiphase, and Adaptive Resolution Platform

The advanced library now exports `continuum_reality_platform.hpp`, providing moving-boundary free-surface CFD, a RANS-transition-LES-DES hierarchy, porous-electrode electrochemistry, two-fluid boiling/condensation/cavitation, participating-media radiation, 3-D field assimilation and inversion, poromechanics and terrain interaction, aerosol population balances, automatic manufactured-solution verification, and simulation-wide adaptive-resolution control.

```bash
cmake --build build --target continuum_reality_platform_tests
ctest --test-dir build --output-on-failure \
  -R '^continuum_reality_platform_(unit_tests|source_regression)$'
```

See [`docs/CONTINUUM_REALITY_PLATFORM.md`](docs/CONTINUUM_REALITY_PLATFORM.md) and Chapter 54 of [`docs/MUZIXDIAGSYS_USER_MANUAL.md`](docs/MUZIXDIAGSYS_USER_MANUAL.md).

## Formula One integrated operations, safety, and energy platform

The focused `aesim_formula_one` library now exports
`formula_one_integrated_operations_platform.hpp`. The additive layer provides
spatial pit-crew and garage scheduling, F1 occupant/HANS/egress biomechanics,
team-radio semantics, dynamic recovery agents, spray optics, carbon-brake
thermomechanics, active-aero and ground-effect stability, sustainable-fuel
combustion with turbo rotordynamics, switching-level ERS/EMC, and Bayesian
CFD-tunnel-track aerodynamic fusion.

```bash
cmake --build build --target formula_one_integrated_operations_platform_tests
ctest --test-dir build --output-on-failure \
  -R '^formula_one_integrated_operations_(platform_unit_tests|source_regression)$'
```

See [`docs/FORMULA_ONE_INTEGRATED_OPERATIONS_PLATFORM.md`](docs/FORMULA_ONE_INTEGRATED_OPERATIONS_PLATFORM.md)
and Chapter 55 of the comprehensive user manual.

## Fundamental Physics Platform

The platform includes entropy-consistent coupling, nonlinear structures, surface
chemistry, rarefied-gas transport, phase fields, coupled waves, certified
reduced-order models, runtime-validity supervision, D-optimal sensor placement,
and causal discrepancy localization. The implementation is isolated in the
`aesim_fundamental_physics` library and remains part of the complete
`aesim_advanced` feature surface through a public CMake dependency. This keeps
focused builds and qualification runs independent of unrelated advanced
subsystems.

```bash
cmake -S . -B build/fundamental \
  -DCMAKE_BUILD_TYPE=Release \
  -DBUILD_TESTING=ON
cmake --build build/fundamental \
  --target fundamental_physics_platform_tests -j
ctest --test-dir build/fundamental --output-on-failure \
  -R '^fundamental_physics_platform_(unit_tests|source_regression)$'
```

For memory-safety qualification, add `-DAESIM_ENABLE_SANITIZERS=ON` and use a
Clang or GCC Debug build. See
[`docs/FUNDAMENTAL_PHYSICS_PLATFORM.md`](docs/FUNDAMENTAL_PHYSICS_PLATFORM.md).

## Frontier vehicle ecosystem expansion (2026-07-28)

The `aesim_advanced` library now includes
`aesim/advanced/frontier_vehicle_ecosystem_platform.hpp`, providing standards-
aware EMC qualification, MATLAB/Simulink and HIL exchange, JAX/PyTorch bridges,
heavy commercial vehicles, WEC/IMSA endurance racing, GIS/photogrammetry,
sensor contamination and cleaning, motorcycle/rider dynamics, population-
resolved occupants, traffic federation, pass-by noise, automated parking,
peridynamics/LBM/BEM/IGA, tire-particle environmental fate, and Formula E,
rally, MotoGP, and drag-racing profiles. See
`examples/frontier_vehicle_ecosystem/README.md` and
`FRONTIER_VEHICLE_ECOSYSTEM_IMPLEMENTATION_REPORT_2026-07-28.md`.

## Electronics engineering and assurance expansion (2026-07-28)

The `aesim_advanced` library now exports three additive electronics platforms:

- `electronics_power_distribution_platform.hpp` for nonlinear low-voltage power networks, priority load shedding, smart fuses, sleep/wake behavior, PMIC/system-basis-chip rail sequencing, and HV precharge/disconnect safety.
- `electronics_circuit_conversion_platform.hpp` for analog/mixed-signal electronics, ADC/DAC nonidealities, PCB SI/PI, ECAD import, grounding/shielding, Si/SiC/GaN/IGBT devices, gate drivers, double-pulse qualification, onboard chargers, isolated DC/DC, wireless charging, and CAN/LIN/Ethernet T1 physical layers.
- `embedded_electronics_assurance_platform.hpp` for bootloaders and flashing, AUTOSAR BSW/MCAL, RTL/SystemC-style co-simulation, LBIST/MBIST, NVM reliability, semiconductor aging, PCBA production, AOI/AXI/ICT, secure provisioning, physical attacks, EMC instrumentation, and automated mitigation.

```bash
cmake --build build --parallel --target \
  electronics_power_distribution_platform_tests \
  electronics_circuit_conversion_platform_tests \
  embedded_electronics_assurance_platform_tests
ctest --test-dir build --output-on-failure \
  -R '^(electronics_power_distribution|electronics_circuit_conversion|embedded_electronics_assurance)_platform_unit_tests$'
```

See [`docs/ELECTRONICS_ENGINEERING_ASSURANCE_PLATFORM.md`](docs/ELECTRONICS_ENGINEERING_ASSURANCE_PLATFORM.md), Chapter 61 of the user manual, and [`examples/electronics_engineering_assurance/`](examples/electronics_engineering_assurance/).

## NHRA championship, strategy, and Heritage expansion (2026-07-29)

The additive `NhraChampionshipStrategyPlatform` provides current-rule-profile championship and event intelligence without replacing the existing generalized drag-racing model:

- Mission Foods regular-season and Countdown event points;
- Lucas Oil national, regional, and divisional eligibility and best-finish selection;
- Countdown point resets, Mission-bonus carry-in, and title-probability simulation;
- Mission #2Fast2Tasty semifinal rematches, final resolution, and 3/2/1 bonus allocation;
- constrained crew-chief tune-up optimization;
- telemetry-driven causal run diagnosis and counterfactual elapsed time;
- round-resolved Monte Carlo event strategy with points, reliability, and US-dollar component cost;
- historical-event and NHRA Hot Rod Heritage profile validation.

```bash
cmake --build build --parallel --target \
  nhra_championship_strategy_platform_tests \
  muzixdiagsys_advanced_platform

./build/muzixdiagsys_advanced_platform nhra capabilities
./build/muzixdiagsys_advanced_platform nhra countdown_simulation \
  examples/nhra_championship_strategy/countdown.json \
  build/nhra-countdown.json build/nhra-evidence
```

See [`docs/NHRA_CHAMPIONSHIP_STRATEGY_PLATFORM.md`](docs/NHRA_CHAMPIONSHIP_STRATEGY_PLATFORM.md), Chapter 62 of the user manual, and [`examples/nhra_championship_strategy/`](examples/nhra_championship_strategy/).

## Global frontend-neutral UI architecture

The simulator now includes `aesim/app/global_ui_architecture.hpp`, an additive architecture for modular domain providers, typed context objects and deep links, Project Explorer and Inspector views, rich unit-aware forms, graph workflows, unified jobs and activity, schema-versioned workspace restoration, linked dashboard layouts, comparison/merge/undo operations, cell-span incremental rendering, large-session virtualization, UI performance instrumentation, and advanced accessibility narration. See `docs/GLOBAL_UI_ARCHITECTURE.md`.

## 2026-08-07 Simulation Assurance, Resilience, and Reproducibility Framework

The industrial assurance stack now includes a unified production framework for deterministic chaos/fault injection, hierarchical SHA-256-verified checkpoints with transactional rollback, structured error taxonomy and causal provenance, dynamic cross-subsystem conservation accounting, confidence-aware numerical evidence, dependency-aware semantic result caching with incremental recalculation, and tamper-evident run certificates. Production industrial commands are guarded by the deterministic fault engine, while assurance/recovery commands remain reachable so a fault campaign cannot lock an operator out of recovery controls.

The command line remains the authoritative interface. Beginner F7/Alt-M menus expose additive assurance entries that generate the same `industrial assurance ...` commands rather than a separate execution path. See [`docs/SIMULATION_ASSURANCE_RESILIENCE_REPRODUCIBILITY.md`](docs/SIMULATION_ASSURANCE_RESILIENCE_REPRODUCIBILITY.md).

## Motorsport CLI convenience commands (Formula One, NASCAR, IndyCar)

The advanced-platform executable and the primary authenticated `muzixdiagsys` interactive shell now share one in-process motorsport dispatcher. Existing command families remain unchanged. The public NASCAR ecosystem, frontier, and next-generation façades are also first-class CLI roots rather than being reachable only through the 40-domain `nascar` aggregate.

```bash
./build/full/muzixdiagsys_advanced_platform f1 capabilities
./build/full/muzixdiagsys_advanced_platform f1 run regulatory full-field-competition \
  examples/formula_one_regulatory_competition/full_field_competition.json build/f1-race.json

./build/full/muzixdiagsys_advanced_platform nascar all-capabilities
./build/full/muzixdiagsys_advanced_platform nascar-ecosystem capabilities
./build/full/muzixdiagsys_advanced_platform nascar-frontier capabilities
./build/full/muzixdiagsys_advanced_platform nascar-next-generation capabilities
./build/full/muzixdiagsys_advanced_platform nascar run integrated telemetry-assimilation \
  examples/nascar_integrated_fidelity/telemetry_assimilation.json build/nascar-telemetry.json

./build/full/muzixdiagsys_advanced_platform indycar capabilities
./build/full/muzixdiagsys_advanced_platform indycar run integrated ecu-hybrid-control \
  examples/indycar_integrated_fidelity/ecu_hybrid_control.json build/indycar-hybrid.json
```

Direct shortcuts include `f1-race`, `f1-ers`, `f1-scrutineering`, `f1-race-control`, `f1-aero`, `f1-setup`, `f1-wet`, `f1-driver`; `nascar-pack`, `nascar-race-control`, `nascar-pit`, `nascar-tyres`, `nascar-setup`, `nascar-racecraft`, `nascar-telemetry`, `nascar-officiating`; and `indycar-hybrid`, `indycar-pit`, `indycar-radio`, `indycar-setup`, `indycar-tyres`, `indycar-safety`, `indycar-timing`, `indycar-driver`.

See [`docs/MOTORSPORT_CLI_COMMANDS.md`](docs/MOTORSPORT_CLI_COMMANDS.md) and Chapter 69 of the comprehensive user manual for the exact syntax, routing map, examples, evidence behavior, and regression commands.

## Advanced API CLI engineering command registry (2026-08-08)

The advanced-platform executable now exposes **214 additional engineering commands** that route directly to existing production C++ APIs across digital thread/calibration, crash/lifecycle, electronics, materials, fundamental physics, real-time/AUTOSAR, scientific computing, measurement/debugging, distributed simulation, deep engineering, fleet/autonomy, silicon/human systems, vehicle ecosystems, and frontier compute.

```bash
./build/full/muzixdiagsys_advanced_platform commands
./build/full/muzixdiagsys_advanced_platform commands --category physics
./build/full/muzixdiagsys_advanced_platform describe credibility
./build/full/muzixdiagsys_advanced_platform credibility self-test \
  build/credibility-self-test build/credibility-self-test.json --profile --explain
./build/full/muzixdiagsys_advanced_platform mdf self-test build/mdf build/mdf.json
./build/full/muzixdiagsys_advanced_platform cfd self-test build/cfd build/cfd.json
```

Every registered command supports `capabilities`, `describe`, `schema`, `example`, `self-test`, and `run`, plus common output/validation controls including JSON/JSONL/CSV/YAML output, evidence directories, deterministic metadata, validation-only/dry-run operation, profiling, trace/metrics sidecars, comparison, timeout qualification, and explanation output. All 214 registry commands are available from the interactive shell as `advanced <command> ...`; non-colliding names are also direct roots. The same direct-export rule now applies to the standalone advanced-platform command families as well, so non-conflicting roots such as `standards`, `emerging`, `frontier-runtime`, `frontier-expansion`, `frontier-systems`, `frontier-integration`, `frontier-next`, `interop`, `rosbag2`, `wireless-phy`, `native-solvers`, `slurm`, and `kubernetes` can be invoked directly from `muzixdiagsys`. Existing simulator roots always retain priority, and the explicit `advanced ...` namespace remains the collision-safe path. Output `-` means stdout, request seed/strict values are reflected in execution metadata, canonical comparison excludes generated timing noise, and substantive compare mismatches fail qualification.

See [`docs/ADVANCED_API_CLI_COMMANDS.md`](docs/ADVANCED_API_CLI_COMMANDS.md), [`examples/advanced_api_cli/`](examples/advanced_api_cli/), and Chapter 70 of the user manual.

### API lifecycle, remote transport, XIL, formal verification, and network services

The lifecycle/transport expansion brought the registry to **194** API-backed command families. It added `api-version`, `api-migrate`, revisioned `api-baseline`, engineering `api-diff`, integrity-checked `api-replay`, `api-lineage`, SHA-256 `artifact-store`, `api-metrics`, OpenTelemetry `api-trace`, native HTTP/2 `grpc-server`, RFC 6455 `telemetry-stream`, `xil-orchestrator`, `formal-reachability`, `wcet`, `schedulability`, `slam`, `network-digital-twin`, `diagnostic-stack`, `road-surface`, `sotif`, and `rss-safety`. All are reachable from the primary `muzixdiagsys` interactive shell and through `advanced <command> ...`. See `docs/API_LIFECYCLE_TRANSPORT_SYSTEM_SERVICES.md` for the complete operations, request semantics, protocol behavior, and examples.

The built-in gRPC service uses real HTTP/2 and Protobuf/gRPC framing through libnghttp2. Full configuration therefore requires the libnghttp2 development headers/library. Windows builds also link the native Winsock and process-status libraries for the transport and metrics services.

### Control, physical-system, co-simulation, and qualification services

The current registry contains **214** API-backed command families. The newest append-only expansion adds `control-synthesis`, `safety-shield`, `prognostics`, `nvh`, `aftertreatment`, `occupant-safety`, `fmi-cosim`, `ssp-orchestrator`, `automotive-middleware`, `charging-session`, `depot-energy`, `ota-campaign`, `digital-key`, `accident-reconstruction`, `tire-digital-twin`, `thermal-management`, `driveline`, `aero-map`, `ads-qualification`, and `probabilistic-model-check`. They reuse production simulator engines and are available directly in the authenticated `muzixdiagsys` shell plus `advanced <command> ...`. See `docs/CONTROL_PHYSICS_COSIM_ENGINEERING_SERVICES.md`.

## Complete backend executable parity in the interactive shell (2026-08-10)

Every non-test backend/tool executable declared by the top-level build now has a fully functional interactive-shell equivalent backed by the **same C++ dispatcher**, not a copied command implementation. The complete mapping is:

| Executable | Interactive command |
|---|---|
| `muzixdiagsys_advanced_platform` | `advanced-platform ...` or `backend advanced-platform ...` |
| `muzixdiagsys_engineering` | `engineering-cli ...` or `backend engineering-cli ...` |
| `muzixdiagsys_causal_lab` | `causal-lab ...` or `backend causal-lab ...` |
| `muzixdiagsys_advanced_safety` | `advanced-safety-cli ...` or `backend advanced-safety-cli ...` |
| `muzixdiagsys_specification_discovery` | `specification-discovery ...` or `backend specification-discovery ...` |
| `muzixdiagsys_standards_deployment` | `standards-deployment ...` or `backend standards-deployment ...` |
| `muzixdiagsys_frontier_professional` | `frontier-professional ...` or `backend frontier-professional ...` |
| `aesim_study_worker` | `study-worker ...` or `backend study-worker ...` |
| `research_reference_generator` | `research-reference-generator ...` or `backend research-reference-generator ...` |

Use `backend list` to inspect the mapping at runtime. Engineering commands invoked inside `muzixdiagsys` inherit the shell's already-authenticated identity/database while retaining the engineering backend's permission checks and tamper-evident audit behavior; no second credential file is required. Standalone `muzixdiagsys_engineering` authentication remains unchanged.

The backend registry now also exports compatibility and executable spellings through the same canonical root resolver (for example `engineering` and `muzixdiagsys_engineering` -> `engineering-cli`) and imports the engineering backend's second-level command grammar into interactive completion. `backend help engineering-cli` lists the live operations and nested paths. These are routing/discovery improvements only: the backend runner remains the single implementation.

The release regression `backend_executable_cli_parity_regression` inventories all nine executable surfaces, checks direct and namespaced completion, runs safe standalone/interactive equivalence probes, verifies byte-identical reference-generator artifacts, validates authenticated engineering-session inheritance, and revalidates the global command schema. See [`docs/BACKEND_EXECUTABLE_CLI_PARITY.md`](docs/BACKEND_EXECUTABLE_CLI_PARITY.md) for the full routing and qualification contract.

## Integrated engineering UI platform (2026-08-10)

The authenticated `muzixdiagsys` shell now includes a shared `ui ...` engineering platform covering terminal-capability negotiation and SGR mouse hit testing, transactional dashboard layout design, a synchronized simulation-time cursor, telemetry/FFT/correlation workbench, network/protocol trace analysis, configuration/result diff and three-way merge, workflow graph authoring, solver diagnostics, CPU/GPU/MPI profiling, experiment/Pareto matrices, SHA-256 evidence browsing, regression triage, automotive four-corner/system/energy views, persistent restorable sessions with observer metadata, Braille/Sixel/Kitty rendering, structured global search, hardened OSC-8/OSC-52 integration, context navigation/pinned inspectors, and an authenticated browser engineering client that routes commands through the canonical shell dispatcher. See [`docs/ENGINEERING_UI_PLATFORM.md`](docs/ENGINEERING_UI_PLATFORM.md).

The professional UI expansion adds five integrated workbenches without replacing any prior surface: **Engineering Mission Control** for jobs/resources/subsystem readiness/alerts, **N-Way Run Comparison** for aligned full-history comparison and envelopes, a **Requirements–Verification–Evidence Matrix** with live SHA-256 staleness detection, a **Design-Space Explorer** operating directly on the experiment matrix, and an automatic **Engineering Flight Recorder** spanning command/result and bounded live-telemetry events. The same canonical commands are available from terminal completion, structured global search, and the authenticated browser workbench.

## V12 Professional Engineering Desktop

V12 adds ten integrated professional engineering workflow surfaces without removing the V11 simulator stack: a schema-driven arbitrary docking/multi-monitor desktop, resumable real-time telemetry streaming, resource-aware campaign orchestration, adaptive DOE/optimization proposals, an executable visual scenario timeline, workflow execution debugging, governed qualification review/approval, live E/E/co-simulation topology, dimension-checked derived telemetry channels, and instrument-grade plot measurements/annotations. All surfaces use the canonical command bus and existing simulation/assurance backends.

Primary V12 command families: `ui desktop`, `ui stream`, `ui campaign`, `ui adaptive-doe`, `ui scenario-timeline`, `ui workflow-debugger`, `ui review-center`, `ui topology`, `ui virtual-channel`, and `ui plot-tools`.

## V13 Professional Engineering Operations

V13 adds a live 3D engineering digital twin, electronic qualification runbooks, change qualification/release planning, a unified engineering data catalog, an interactive calibration/correlation workbench, and real-time collaborative engineering sessions. See `docs/PROFESSIONAL_ENGINEERING_OPERATIONS_V13.md`. All six are exposed through canonical `ui ...` shell commands and preserve the existing backend/API parity contract.

## V16 Graphical Engineering Desktop

V16 upgrades the authenticated browser engineering client into a direct-manipulation desktop over the existing canonical V12/V13/V15 UI models. It adds recursive graphical dock/tab manipulation and floating windows, a real WebGL renderer for `EngineeringDigitalTwinViewport3D`, interactive out-of-core telemetry plotting, a virtualized engineering data grid, graphical calibration-map editing, interactive E/E topology, drag-and-drop/resizable scenario events, visual workflow authoring/debugging, spatial track/lap run comparison, and a graphical Semantic CLI with a consolidated Problems panel.

No simulation, calibration, workflow, scenario, telemetry, access-control, or 3D scene backend is duplicated. Browser mutations are routed through the authenticated canonical command dispatcher. New nested operations are `ui semantic json`, `ui desktop activate`, `ui desktop reorder`, `ui scenario-timeline resize`, `ui workflow-editor json`, `ui workflow-debugger json`, `ui calibration-correlation json`, and `ui run-compare track-json`.

See [`docs/ENGINEERING_UI_PLATFORM.md`](docs/ENGINEERING_UI_PLATFORM.md) and User Manual Chapter 78.

### V18 Browser Engineering Operations

The embedded authenticated web GUI now adds a Live Operations cockpit, persistent signal watchlists with bounded client-side sparklines, workbench search/favorites, System Snapshot, Problems filtering/export, browser telemetry/state downloads, command history, keyboard shortcuts, and dedicated graphical adapters for the existing Command Staging, Macro Library, Incident/First-Out, and Engineering Scratchpad authorities. The browser continues to use only `/api/state`, `/api/schema`, `/api/stream`, and `/api/command`; no feature-specific mutation endpoint or duplicate simulator service was added. See User Manual Chapter 88 and [`docs/ENGINEERING_UI_PLATFORM.md`](docs/ENGINEERING_UI_PLATFORM.md).

## ECM / OBD-II diagnostic digital twin (2026-08-12)

MuzixDiagSys now includes a unified virtual ECM diagnostic executive integrated with the existing ECU strategy, physical plant, canonical `DiagnosticService`, ISO-TP/CAN/CAN-FD stack, SocketCAN/HIL interface, DoIP routing, ELM327 adapter, diagnostic workflow engine, causal graph, and network-fault laboratory. The implementation does not create a competing OBD or UDS stack: the existing diagnostic service remains authoritative and the ECM layer supplies lifecycle, monitor, calibration, flash, fault-propagation, conformance, and campaign orchestration.

Primary interactive commands include:

```text
ecm status
ecm scheduler
ecm provenance [signal]
ecm dtc [all|pending|confirmed|permanent|healed|clear]
ecm monitor [misfire|fuel-system|comprehensive-components|catalyst|oxygen-sensor|evap-system|egr-vvt]
ecm calibration get <name>
ecm calibration set <name> <value>
ecm flash status|enter|erase|download <hex>|verify|activate|interrupt|recover
ecm fault wiring <path> <open|short-ground|short-battery|bias|resistance|drift> <0..1>
ecm fault clear [path|all]
ecm active-test <actuator> <0..100>
ecm root-cause
ecm test-plan <DTC>
ecm obd <hex>
ecm uds <hex>
ecm obdonuds <hex>
ecm wwh <hex>
ecm zev <hex>
ecm doip <UDS-hex>
ecm isotp [fd] <hex>
ecm isotp fault drop|corrupt|duplicate|reorder|sequence|bus-off <N>
ecm j2534 status|write <UDS-hex>
ecm elm <AT-command|OBD-hex>
ecm hil status|enable [interface] [fd]|disable
ecm conformance
ecm fuzz [seed] [cases]
ecm campaign <regulatory|misfire|fuel|catalyst|evap> [cycles] [seed]
```

The `obd` root retains its established live-data/reporting commands and additionally routes DTC lifecycle, readiness/monitor, provenance, conformance, fuzzing, campaign, OBDonUDS, WWH-OBD, and ZEVonUDS operations into the same ECM diagnostic executive.

## Version 20 UI Customization Platform

Version 20 includes a presentation-only UI Customization Platform that composes the existing workspace, dashboard, telemetry, theme, keybinding, workflow, accessibility, resource-governor, browser and terminal UI authorities without changing simulation fidelity. Start with `ui customize status`, `ui customize profile list`, or `ui customize diagnostics activate`. Full reference: `docs/UI_CUSTOMIZATION_PLATFORM.md`.


### V20.1.2 Research-Grade Engineering Workbenches

The Unified Engineering UI now includes 28 additional research-grade workbenches: formal counterexamples, multiphysics field visualization, sparse-Jacobian inspection, distributed tracing/critical path, HPC placement, graphical safety, temporal bisection, live contracts, state machines, numerical error budgets, run lineage, real-time deadline/jitter analysis, co-simulation synchronization, source/requirement/test coverage, cyber attack graphs, engineering notebooks, evidence-linked reports, CRDT collaboration, plugin management, schema migration, dependency heatmaps, automated performance/divergence investigation, regression clustering, digital-twin measurement/sectioning, alert-rule authoring, product-line constraints, and a multi-host control room.

The browser remains a client of canonical interactive-shell commands through `/api/command`; plugin/config/formal/safety/distributed backends are reused rather than duplicated. See `docs/ENGINEERING_UI_PLATFORM.md` and User Manual Chapter 83.

## V20.1.2 integrated terminal engineering cockpit

The authenticated InteractiveShell now exposes terminal-native projections for high-resolution Unicode telemetry sparklines, synchronized event timeline/time travel, causal inspection, experiment cockpit, the existing Mission Control job manager, notifications, tabbed analytical lower-pane views, hierarchical subsystem navigation, parameter inspection, UI undo/redo, inline documentation, motorsport pit wall, terminal track map, friction circle, runtime profiler dashboard, and compact uncertainty display.

Canonical commands include `ui sparkline`, `ui event-timeline`, `ui time-travel`, `ui causal-inspector`, `ui experiment-cockpit`, `ui jobs`, `ui notifications`, `ui lowerpane`, `ui navigator`, `ui parameter-inspector`, `ui undo|redo`, `ui doc-inspect`, `ui pit-wall`, `ui track-map`, `ui friction-circle`, `ui performance-profiler`, and `ui uncertainty-view`. These commands reuse `TelemetryWorkbench`, `SynchronizedTimeCursor`, `EngineeringFlightRecorder`, `CausalDifferenceExplorer`, `ExperimentMatrix`, Mission Control `JobManager`/alerts, `ContextGraph`, `ExperienceManager`, `NWayRunComparisonWorkbench`, and `RuntimeProfiler`; no parallel backend stores were added.

The Command Activity lower-pane remains the default for compatibility. Analytical views can be selected with `ui lowerpane view activity|events|timeline|jobs|notifications|experiments|profiler|navigator|causal`, and the selected view is persisted with UI preferences/project layout metadata. See User Manual Chapter 84 and `docs/ENGINEERING_UI_PLATFORM.md` for exact commands, data semantics, and qualification.

### V20.1.2 TUI readability, terminal selection, and high-resolution meters

The terminal client now leaves application mouse capture **off by default**, so normal terminal drag-selection and copy/paste remain available. `ui mouse on` explicitly enables button/wheel interaction using SGR mouse coordinates without continuous motion reporting; `ui mouse off` releases all application mouse modes. Bracketed paste protection remains enabled. Mouse escape sequences received while capture is off are consumed as no-ops and cannot wedge the InteractiveShell.

Bounded progress/status meters now share `aesim::core::terminal_visuals::high_resolution_bar()` and use eighth-cell Unicode block resolution rather than `#` fill characters. Existing telemetry sparklines are intentionally unchanged because they represent time history, not bounded completion. Status-row groups and scenario timelines also use clearer Unicode separators/markers while preserving established PTY-visible command/status anchors.

See [`docs/REAL_WORLD_TUI_USAGE_GUIDE.md`](docs/REAL_WORLD_TUI_USAGE_GUIDE.md) for simple real-world examples and explanations.

## Professional Operator TUI — 93-feature qualification generation

The terminal UI now adds statistical run-family envelopes, semantic “why highlighted” explanations, live what-changed ranking, metric provenance graphs, control hysteresis visualization, state-transition ribbons, SOE alarm-flood/chatter analysis, incident workspace generation, pane maximize/restore, per-layout responsive breakpoints, the persistent semantic command-path ribbon, atomic staged-command rollback, a unit-aware engineering scratchpad, production frame-jank capture, and live requirement margins. These features reuse the existing run-comparison, telemetry, state-machine, SOE, workspace/pane, semantic CLI/transaction, virtual-channel/unit, performance, and requirements/verification authorities rather than duplicating them. See User Manual Chapter 87 for command syntax, ownership rules, and engineering workflows.


### V19 Integrated Engineering Analysis Desktop

The authenticated web desktop now provides a shared engineering-analysis context across Requirements & Evidence, N-Way Run Comparison, Regression Divergence, Engineering Event Timeline, State Machine, Diagnostic Center, Solver Observability, Calibration Correlation, Artifact/Evidence, Reproducibility, and Qualification workbenches. Selecting a requirement, signal, run, event, state, diagnostic causal node, artifact, calibration cell, or runtime resource publishes one browser-wide selection context. Primary/A/B time cursors are synchronized through the existing `ui linked-cursor` authority; browser follow-live mode periodically synchronizes the primary cursor without creating a second time model.

V19 also adds graphical requirements/evidence matrices with live margins, multi-run overlays and statistics, first-divergence navigation, SOE timeline inspection, state-machine graph debugging, a diagnostic causal DAG, resource/solver observability, calibration change review with semantic access preflight and the existing stage/approve workflow, artifact evidence browsing, reproducibility-manifest aggregation, an engineering qualification dashboard, role-aware command affordances, and automatic structured rendering for canonical JSON command results. The browser continues to expose only `/api/state`, `/api/schema`, `/api/stream`, and `/api/command`; mutations continue through the canonical shell dispatcher and existing permission/transaction authorities. See User Manual Chapter 89 and [`docs/ENGINEERING_UI_PLATFORM.md`](docs/ENGINEERING_UI_PLATFORM.md).


## Connected Vehicle Integration Platform (2026-08-17)

The additive `aesim::advanced::connected` platform adds eight integrated research subsystems without replacing existing NR-V2X, AUTOSAR/realtime, camera, battery, cybersecurity, networking, or compute functionality:

- J2735 BSM/SPaT/MAP/PSM/TIM application-message modeling with IEEE 1609.2-oriented P-256 signing, PSID policy, revocation, freshness, and replay defense.
- DDS Security / SROS2 governance, permissions, identities, AES-256-GCM transport, signed samples, and replay protection.
- RAW Bayer/HDR camera ISP with black-level, shading, bad-pixel, denoise, demosaic, AWB, CCM, tone map, sharpening, gamma, and auto-exposure.
- DMS/OMS sensor digital twin with PERCLOS, distraction/drowsiness, liveness, seat/child/respiration/belt fusion.
- RTOS execution co-simulation with preemption, multicore dispatch, mutexes, priority inheritance, deadlines, response/blocking metrics, and trace evidence.
- PCIe/CXL central-compute timing with IOMMU/TLB, SR-IOV, AER, contention, coherent transactions, and DMA/MMIO.
- Wireless BMS RF/electrothermal/estimation loop with fading, interference/jamming, retries, balancing, degraded estimation, and safety decisions.
- LTE/5G NR/NTN telematics modem with eSIM roaming, registration, handover, QoS, sleep, throughput/latency, power, and thermal throttling.

See `docs/CONNECTED_VEHICLE_INTEGRATION_PLATFORM.md`. The focused native test target is `connected_vehicle_integration_platform_tests`; source-retention hardening is provided by `tests/connected_vehicle_integration_source_regression.py`.

## 2026-08-17 V20.1.2 Physical Diagnostics and Intelligence Platform

V20.1.2 now extends the existing multimodal renderer with deterministic indexed-mesh BVH acceleration shared by camera, thermal, lidar, and FMCW radar; extends the crash lifecycle with pedestrian/cyclist/motorcyclist VRU biomechanics; and adds experimental NVH FRF/TPA/OMA/modal correlation, friction-induced brake-squeal stability analysis, defect-driven rolling-bearing diagnostics/prognostics, shifted-Heaviside XFEM fracture/fatigue propagation, persistent SHA-256 experiment/artifact lineage DAGs, and PC/FCI/GES/NOTEARS/PCMCI causal discovery. Existing renderer, occupant crash, bearing mechanics, fracture, provenance, and causal-runtime features remain authoritative and are extended rather than duplicated. See `docs/PHYSICAL_DIAGNOSTICS_INTELLIGENCE_PLATFORM.md` and `PHYSICAL_DIAGNOSTICS_INTELLIGENCE_IMPLEMENTATION_REPORT_2026-08-17.md`.

## Engineering Validation Platform (V20.1.2)

The V20.1.2 engineering-validation expansion adds commercial tire parameter identification, measured-vs-simulated test correlation and road-load reconstruction, governed domain-randomized sim-to-real qualification, optimized grid-aware charging, checkpointed optimistic/conservative PDES, operating-domain credibility scoring, interface-attributed conservation diagnostics, and a generalized lubrication hydraulic supply network. See `docs/ENGINEERING_VALIDATION_PLATFORM.md` for the full API and non-duplication architecture.

## Terminal Workstation Platform

The V20.1.2 terminal UI includes a multi-pane engineering workstation with a virtualized grid, Scientific Scope 2.0, adaptive SSH rendering, schema-driven command forms, triggered incident capture, professional alarm lifecycle, presentation-unit profiles, plugin pane registration, artifact inspection, synchronized multi-run comparison, terminal qualification, investigation notebooks, semantic context actions, and workspace automation.  See `docs/TERMINAL_WORKSTATION_PLATFORM.md`.

### Terminal Engineering IDE Expansion (2026-08-18)

The Terminal Workstation now includes unified engineering-graph/dataflow navigation, calibration surface selection/editing, experiment composition, deterministic TUI session recording/replay, HPC/PDES operations, fault/falsification orchestration, universal telemetry/evidence querying, qualification and flamegraph views, persistent remote sessions, sensitivity inspection, cross-domain timeline 2.0, build diagnostics, HIL operations, field-slice heatmaps, and semantic accessibility.  These are terminal orchestration/presentation extensions over the existing `ContextGraph`, calibration studio, experiment matrix, session registry, diff/merge, design-space, distributed trace, multiphysics field, HIL, and canonical command infrastructures; they do not introduce duplicate authorities. See `docs/TERMINAL_WORKSTATION_PLATFORM.md`.
