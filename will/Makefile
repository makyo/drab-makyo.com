.PHONY: all
all: signed-will.md.asc notifications.md.asc

signed-will.md.asc: will.md
	gpg -o signed-will.md.asc -sa will.md

notifications.md.asc: notifications.md
	gpg -o notifications.md.asc -sa notifications.md
