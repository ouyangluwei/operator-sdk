---
title: "operator-sdk cleanup"
---
## operator-sdk cleanup

Delete and clean up after a running Operator

### Synopsis

Delete and clean up after a running Operator

```
operator-sdk cleanup [flags]
```

### Options

```
      --kubeconfig string           The file path to kubernetes configuration file. Defaults to location specified by $KUBECONFIG, or to default file rules if not set
      --namespace string            (Deprecated: use --operator-namespace instead.) The namespace from which operator and namespacesresources are cleaned up
      --olm                         The operator to be cleaned up is managed by OLM in a cluster. Cannot be set with another cleanup-type flag (default true)
      --olm-namespace string        [olm only] The namespace where OLM is installed (default "olm")
      --operator-namespace string   [olm only] The namespace where operator resources are created. It must already exist in the cluster or be defined in a manifest passed to --include
      --install-mode string         [olm only] InstallMode to create OperatorGroup with. Format: InstallModeType[=ns1,ns2[, ...]]
      --timeout duration            [olm only] Time to wait for the command to complete before failing (default 2m0s)
      --manifests string            [olm only] Directory containing operator package directories and a package manifest file
      --operator-version string     [olm only] Version of operator to deploy
      --include strings             [olm only] Path to Kubernetes resource manifests, ex. Role, Subscription. These supplement or override defaults generated by run/cleanup
  -h, --help                        help for cleanup
```

### SEE ALSO

* [operator-sdk](../operator-sdk)	 - An SDK for building operators with ease

