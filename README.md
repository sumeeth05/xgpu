**xgpu** is a minimal, explicit, cross-platform GPU abstraction layer for modern graphics APIs.

It provides a clean and unified interface over Vulkan, DirectX 12, Metal, and other backends while staying close to the underlying hardware. xgpu is designed for developers who want full control over GPU execution without the verbosity of raw APIs or the hidden behavior of high-level frameworks.

The API is intentionally small and explicit: command encoding, resource creation, and submission are all user-driven, with no implicit state, automatic pipelines, or hidden synchronization. This ensures predictable behavior and near-native performance.

xgpu supports both 2D and 3D rendering workflows and includes optional ray tracing through a separate module, allowing access to advanced features without overcomplicating the core API.

This crate is not a game engine or renderer. It is a thin abstraction layer that organizes GPU work while preserving control, performance, and clarity.

**Key features:**

- Cross-platform: Vulkan, DirectX 12, Metal (and optional fallbacks)
- Explicit command-based API (no hidden work)
- Minimal, consistent interface across backends
- Near-native performance with low overhead
- Optional ray tracing support
- Designed for building renderers and graphics systems from scratch
