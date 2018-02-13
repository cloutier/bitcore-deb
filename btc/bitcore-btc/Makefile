all:
	git clone https://github.com/satoshilabs/bitcore
	cd bitcore && git checkout 982c6c9c01a036193f55b25efa3090b143f03f54
	cd bitcore && rm -rf .git # Delete .git folder to reduce space
	cd bitcore && yarn
	rm -rf bitcore/node_modules/bitcore-node/bin/*.gz
	rm -rf bitcore/node_modules/bitcore-node/bin/bitcoin-*/bin/bitcoin-qt
	rm -rf bitcore/node_modules/bitcore-node/bin/bitcoin-*/bin/test_bitcoin
	rm -rf bitcore/node_modules/bitcore-node/test/*
	git clone https://github.com/cloutier/insight.git
	cd insight && git checkout catallaxy
	rm -rf bitcore/node_modules/insight-ui
	ln -s bitcore/node_modules/insight-ui insight


clean:
	rm -fr bitcore
