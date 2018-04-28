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

.PHONY: new-1-awesome
new-1-awesome:
	cp -r 0-original 1-awesome
	cd 1-awesome && mkdir data

.PHONY: rm-1-awesome
rm-1-awesome:
	rm -rf 1-awesome

.PHONY: patch-1-awesome
patch-1-awesome:
	cp -r 1-awesome-patch/.vuepress/* 1-awesome/.vuepress
	cp -r 1-awesome-patch/*.md 1-awesome
	cp -r 1-awesome-patch/data/* 1-awesome/data