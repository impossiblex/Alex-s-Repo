# platform-engineering


# Deploy

	docker login ghcr.io --username dubadub --password-stdin

	docker build -t ghcr.io/impossiblex/paleo.io-web:0.0.1 .
	docker push  ghcr.io/impossiblex/paleo.io-web:0.0.1

	ansible-playbook playbooks/deploy_paleo.io.yml -i inventory/hosts
