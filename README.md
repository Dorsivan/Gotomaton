## Our First Mission

### Mission 1

we need to construct a go code that recieves a go.mod file, downloads EVERY requirement it has (so, the dependencies) and bundles them into a tar!

This requires research! Yes, this isn't too complicated, but this is only the start. First you gotta verify where all of this downloads too, then select only the files we need as dependencies, then we bundle them into a tar.

Go can work with local dependencies. This means that for you to make sure, you will need to use them locally and make sure it works properly.

Afterwards, we will have more missions. This is mostly for you to learn golang for a start, so that we can move into cdk8s.

aye?

```
module example.com/cdk8s-demo

go 1.16

require (
	github.com/aws/constructs-go/constructs/v10 v10.1.123
	github.com/aws/constructs-go/constructs/v3 v3.4.115
	github.com/aws/jsii-runtime-go v1.69.0
	github.com/cdk8s-team/cdk8s-core-go/cdk8s v1.8.7
	github.com/cdk8s-team/cdk8s-core-go/cdk8s/v2 v2.5.8
)
```

pro tip, dont forget about such commands like `go mod tidy` and `go mod graph`