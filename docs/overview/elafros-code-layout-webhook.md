# Code layout - Webhook

* `./pkg/webhook/webhook.go`
  * All the generic mutations / validations
  * Serialization / deserialization
* Calls into resource specific validation / mutation
  * `./pkg/webhook/{configuration,revision,route,service}`
* Mutations specified with an array of jsonpatch objects
* `./pkg/webhook/certs.go`
  * CA / Server cert 

