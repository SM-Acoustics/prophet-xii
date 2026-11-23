
## Agentic software-assurance checklist
- [ ] AI assistance and exact changed modules disclosed
- [ ] Requirement/source, affected production entry point and reachability recorded
- [ ] New stubs/TODO/dead code audited; unsupported work fails explicitly
- [ ] Independent reference/oracle plus negative/edge/regression evidence provided
- [ ] No tests, gate, CI or security checks silently weakened
- [ ] Unsafe/FFI, DMA/MMIO, concurrency, allocations, deadlines and supply chain reviewed where applicable
- [ ] Capability status (UNSUPPORTED / IMPLEMENTED_UNVERIFIED / VERIFIED / FAILED) and exact HOST/QEMU/DEVICE scope stated
- [ ] Commands, targets, versions, failure receipts, hashes and residual risks provided
- [ ] No hardware action, merge, deployment or release without human approval
