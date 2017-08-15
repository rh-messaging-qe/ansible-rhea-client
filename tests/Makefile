.PHONY: package_install clean

# name of containers from inventory
containers = aron deca thor

all: scenario1

scenario1:
	docker rm -f $(containers) || true
	ansible-playbook -i inventory playbook_install_scenario.yml

clean:
	docker rm -f $(containers) || true
