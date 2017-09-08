.PHONY: package_install clean

# name of containers from inventory
containers = zeus hades

all: scenario1

scenario1:
	docker rm -f $(containers) || true
	ansible-playbook -i hosts test_main.yml

clean:
	docker rm -f $(containers) || true
