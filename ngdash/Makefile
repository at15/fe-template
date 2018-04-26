.PHONY: new-empty
new-empty:
# https://github.com/angular/angular-cli/wiki/new
	ng new empty --routing=true

.PHONY: rm-empty
rm-empty:
	rm -rf empty

# https://github.com/NG-ZORRO/ng-zorro-antd
.PHONY: new-zorro
new-zorro:
	cp -r empty zorro
	cd zorro && npm install ng-zorro-antd@0.7.0-beta.4 --save

.PHONY: rm-zorro
rm-zorro:
	rm -rf zorro

.PHONY: patch-zorro
patch-zorro:
	cp -r zorro-patch/* zorro
# need to include default theme from ng-zorro, they are using less
	cp zorro-patch/.angular-cli.json zorro