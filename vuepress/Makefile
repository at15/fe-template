.PHONY: new-empty
new-empty:
# https://vuepress.vuejs.org/guide/getting-started.html
	mkdir empty
	make patch-empty
	cd empty && npm install -D vuepress

.PHONY: rm-empty
rm-empty:
	rm -rf empty

.PHONY: patch-empty
patch-empty:
	cp -r empty-patch/* empty
	cp -r empty-patch/.vuepress empty