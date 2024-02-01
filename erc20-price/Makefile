.PHONY: build
build:
	cargo build --target wasm32-unknown-unknown --release

.PHONY: run
run:
	substreams run -e eth.substreams.pinax.network:443 substreams.yaml map_eth_price -s -10 

.PHONY: pack
pack:
	substreams pack ./substreams.yaml --output-file target/erc20-price-substreams-v0.1.0.spkg