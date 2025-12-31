# https://github.com/aws-cloudformation/cfn-lint
# https://github.com/aws-cloudformation/rain

all: lint fmt

lint:
	cfn-lint github-oidc-cloudformation.yml
	cfn-lint service-account-cloudformation.yml

fmt:
	rain fmt --write github-oidc-cloudformation.yml
	rain fmt --write service-account-cloudformation.yml
