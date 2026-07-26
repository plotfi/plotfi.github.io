# Puyan Lotfi - Resume Links

Reference page for links cited in my resume.

## Triton / GPU compiler work (Meta, 2018-present)

| Link | What it is |
| --- | --- |
| [Triton Plugin Extensions: Enabling TLX and Custom Compiler Passes Out of the Box](https://pytorch.org/blog/triton-plugin-extensions-enabling-tlx-and-custom-compiler-passes-out-of-the-box/) | PyTorch blog, July 2026. Co-authored. The writeup of the Triton plugin extension system shipped in Triton 3.7, and of `utlx` as its first major consumer. Covers the overridable pass pipeline, custom dialects and DSL ops, and cross-vendor results on H100 and MI350. |
| [Fast 2-Simplicial Attention: Hardware-Efficient Kernels in TLX](https://pytorch.org/blog/fast-2-simplicial-attention-hardware-efficient-kernels-in-tlx/) | PyTorch blog, September 2025. Not authored by me; cited as the reference result for the TLX technique set that µTLX brings to upstream Triton. |
| [triton-utlx on PyPI](https://pypi.org/project/triton-utlx/) | The µTLX plugin package, installable against unmodified upstream Triton. |
| [BF16xN benchmark log](https://gist.github.com/plotfi/72554bd410ea55d8ae67b501c69b2766) | Raw tritonbench tutorial-matmul numbers behind the BF16x3 result: 69.1 to 112.9 TFLOPs average over 256-4096 square GEMMs, +63% over the default IEEE FP32 path. Also shows BF16x6 at +10% and BF16x9 at -7%. |

## Swift C++ interoperability (Meta)

| Link | What it is |
| --- | --- |
| [Swift C++ Interoperability Workgroup](https://bit.ly/3zfY3YF) | **Destination to confirm.** Swift forums thread for the C++ interop workgroup, where I served as Meta's representative. |
| [C++ / Objective-C interop issues](https://bit.ly/3hJhimH) | **Destination to confirm.** Cross-company working group thread on C++/Objective-C interop problems. |
| [cxx-interop-diff](https://github.com/plotfi/cxx-interop-diff) | Tooling I wrote to diff Swift's ingestion of every Apple framework with C++ interop enabled and disabled. |

## Clang / LLVM (Meta)

| Link | What it is |
| --- | --- |
| [Objective-C direct ABI RFC](https://bit.ly/4wQYRO2) | **Destination to confirm.** My RFC for the Objective-C direct ABI, which seeded the later upstreaming effort. |
| [Clang Interface Stubs lightning talk](https://bit.ly/35ap4uk) | **Destination to confirm.** 2019 LLVM Developers' Meeting lightning talk on Clang Interface Stubs / llvm-ifs. |
| [Fuchsia adoption commit](https://fuchsia.googlesource.com/fuchsia/+/5e786c3) | Google's Fuchsia OS picking up llvm-ifs / Clang Interface Stubs. |

## Apple GPU work (2013-2018)

| Link | What it is |
| --- | --- |
| [US Patent 10310830](https://patents.google.com/patent/US10310830B2) | GPU shader profiling. Granted for the binary-level shader analysis library behind the Metal Shader Profiler. |
| [Optimizing Performance with the Shader Profiler](https://developer.apple.com/documentation/metal/gpu_functions_libraries/optimizing_performance_with_the_shader_profiler) | Apple developer documentation for the Metal Shader Profiler, shipped in Xcode 10, which integrated my analysis library. |
| [Improving Code Diff Through Canonical Transformation](https://youtu.be/RHT-bh_xo6U) | EuroLLVM 2018 talk on MIR-Canon. |

## Elsewhere

| Link | What it is |
| --- | --- |
| [github.com/plotfi](https://github.com/plotfi) | Upstream LLVM, Clang, and Triton contributions. |
| [puyan.org](https://www.puyan.org) | Home page. |

---

### Notes before publishing

- The four **destination to confirm** rows are bit.ly shorteners whose targets I could not resolve. Replace each with its canonical URL before hosting, and update the resume to match. Once this page exists, the resume can drop the inline shorteners and cite `puyan.org/links` instead.
- The PyPI and gist rows are not currently cited on the resume. Included because they are the primary evidence for two of its claims.
- Anything internal-only (the RFC, if it was never posted publicly) should either be removed or marked as internal rather than linked.
