HUBUSER ?= "jbournepers"
REPONAME ?= "rocky9-toolbox"
VERSION ?= "1.5"

all: build push

build:
	docker build --no-cache -t "$(HUBUSER)/$(REPONAME):$(VERSION)" .

push:
	docker push "$(HUBUSER)/$(REPONAME):$(VERSION)"

clean:
	rm -f *~
	docker image rm "$(HUBUSER)/$(REPONAME):$(VERSION)"

