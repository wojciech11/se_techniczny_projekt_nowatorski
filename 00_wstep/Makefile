DECKTAPE_VERSION=3

# npm install decktype
# node node_modules/decktape/decktape.js -s 2560x1600 index.html index.pdf
give_me_pdf:
	docker run --rm -v $$(pwd):/slides \
		--platform linux/amd64 \
		-v $$(pwd):/home/user astefanutti/decktape:$(DECKTAPE_VERSION) \
		-s 2560x1600 index.html index.pdf

give_me_zip:
	cd .. && zip -r $(CURDIR).zip $(CURDIR)/*

