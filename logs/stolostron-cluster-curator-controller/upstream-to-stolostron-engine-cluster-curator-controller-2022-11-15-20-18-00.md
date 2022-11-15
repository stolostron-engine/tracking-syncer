## Syncing stolostron/cluster-curator-controller with stolostron-engine/cluster-curator-controller

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 1 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
3964e5e0d3ca6e768b40e4e6a82e5307cae6298b Add HookType to distinguish Job or Workflow. If the type is empty or Job then the controller will create AnsibleJob with Spec.job_template_name as the key. If the type is Workflow then the AnsibleJob will use Spec.workflow_template_name instead. (#137)
```

Status: Syncing successful
