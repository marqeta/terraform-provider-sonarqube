# sonarqube_qualitygate
Provides a Sonarqube Quality Gate resource. This can be used to create and manage Sonarqube Quality Gates.

## Example: create a quality gate
```terraform
resource "sonarqube_qualitygate" "main" {
    name = "example"
    is_default = true
}
```

## Argument Reference
The following arguments are supported:

- name - (Required) The name of the Quality Gate to create. Maximum length 100
- is_default - (Optional) When set to true this will make the added Quality Gate default

## Attributes Reference
The following attributes are exported:

- name - Name of the Sonarqube Quality Gate
- id - ID of the Sonarqube Quality Gate

## Import 
Quality Gates can be imported using their numeric value

```terraform
terraform import sonarqube_qualitygate.main 11
```

