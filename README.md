# Terraform Resources
A collection of Terraform resources

- https://medium.com/spaceapetech/creating-a-terraform-provider-part-1-ed12884e06d7
- https://github.com/spaceapegames/terraform-provider-example

Creating a Terraform Provider

`Terraform Plugins are binaries that Terraform communicates with via RPC.`

- All providers start with terraform-provider-
- Entry point is `main.go`
- Create a `provider` package in `provider.go` and define `func Provider() terraform.ResourceProvider` function

There are 3 things the provider requires:
1. Schema: attributes
2. ResourcesMap: defines resoure names
3. ConfigureFunc: any setup
