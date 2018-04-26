.PHONY: new-0-original
new-0-original:
# https://vuepress.vuejs.org/guide/getting-started.html
	mkdir 0-original
	cd 0-original && npm install --save-dev vuepress

.PHONY: rm-0-original
rm-0-original:
	rm -rf 0-original

.PHONY: patch-0-original
patch-0-original:
	cp -r 0-original-patch/package.json 0-original
	cp -r 0-original-patch/README.md 0-original
	cp -r 0-original-patch/.vuepress 0-original/.vuepress

.PHONY: sync-0-original
sync-0-original:
	cp -r 0-original-patch/README.md 0-original
	cp -r 0-original-patch/.vuepress/* 0-original/.vuepress