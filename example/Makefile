# features/Makefile
ROLES_PATH := roles
REQUIREMENTS := requirements.yml

.PHONY: install clean

install:
	@echo "==> Встановлення Ansible ролей з Galaxy..."
	ansible-galaxy install -r $(REQUIREMENTS) -p $(ROLES_PATH) --force
	@echo "==> Готово."

clean:
	@echo "==> Видалення встановлених ролей..."
	rm -rf $(ROLES_PATH)/devsec.os_hardening
	rm -rf $(ROLES_PATH)/devsec.ssh_hardening
	rm -rf $(ROLES_PATH)/geerlingguy.security
	@echo "==> Готово."