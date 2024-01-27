.PHONY: clean

clean:
	@echo "Cleaning previous build"
	@cargo clean

.PHONY: rebuild

rebuild:
	@echo "Cleaning previous build"
	@cargo clean
	@echo "Running cargo xtask build-ebpf..."
	@cargo xtask build-ebpf
	@echo "Running cargo build..."
	@cargo build
	@echo "Running RUST_LOG=info cargo xtask run..."
	@RUST_LOG=info cargo xtask run
