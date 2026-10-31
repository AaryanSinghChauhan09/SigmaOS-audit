# SigmaOS Audit

An evolving `no_std` Rust library for audit-related data structures and policy prototypes. The crate exposes `AuditManager`; the audit module defines event and severity types and includes memory-audit and process-pledge code.

The source alone does not establish complete page-table inspection, durable audit logging, process-isolated policy enforcement, trusted timestamps, or production-ready security monitoring. Review the implementation and its integration before relying on it as a security control.

## Build

The manifest references sibling [`SigmaOS-kernel`](../SigmaOS-kernel) and [`SigmaOS-security`](../SigmaOS-security) crates. From the SigmaOS checkout:

```sh
cargo check --manifest-path SigmaOS-audit/Cargo.toml --lib
```

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
