# https://github.com/aws-cloudformation/cfn-lint

STACK_NAME := iac-$(shell git rev-parse --short HEAD)
PARAMS = GitHubRepository=automate6500/lambda-cicd

lint:
	cfn-lint terraform-service-account-cloudformation-template.yml

deploy:
	rain deploy terraform-service-account-cloudformation-template.yml $(STACK_NAME) \
		--yes --params $(PARAMS)

