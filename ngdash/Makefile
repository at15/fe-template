.PHONY: new-empty
new-empty:
	ng new empty

# https://github.com/NG-ZORRO/ng-zorro-antd
.PHONY: new-ngzorro
new-ngzorro:
	cp -r empty zorro
	cd zorro && npm install ng-zorro-antd --save

.PHONY: patch-ngzorro
patch-ngzorro:
	cp -r zorro-patch/* zorro