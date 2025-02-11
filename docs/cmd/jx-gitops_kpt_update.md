## jx-gitops kpt update

Updates any kpt packages installed in a sub directory

### Usage

```
jx-gitops kpt update
```

### Synopsis

Updates any kpt packages installed in a sub directory 

If you know a specific directory which needs updating you can always use 'kpt' directly via: 

          kpt pkg update mySubDir

### Examples

  # recurses the current dir looking for directories with Kptfile inside
  # and upgrades the kpt package found there to the latest version
  jx-gitops kpt --dir .

### Options

```
      --bin string          the 'kpt' binary name to use. If not specified this command will download the jx binary plugin into ~/.jx3/plugins/bin and use that
      --dir string          the directory to recursively look for the *.yaml or *.yml files (default ".")
  -h, --help                help for update
      --ignore-yaml-error   ignore kpt errors of the form: yaml: did not find expected node content
  -o, --owner string        filter on the Kptfile repository owner (user/organisation) for which packages to update
  -r, --repo string         filter on the Kptfile repository name  for which packages to update
  -s, --strategy string     the 'kpt' strategy to use. To see available strategies type 'kpt pkg update --help'. Typical values are: resource-merge, fast-forward, alpha-git-patch, force-delete-replace (default "alpha-git-patch")
  -u, --url string          filter on the Kptfile repository URL for which packages to update
  -v, --version string      the git version of the kpt package to upgrade to
```

### SEE ALSO

* [jx-gitops kpt](jx-gitops_kpt.md)	 - Commands for working with kpt packages

###### Auto generated by spf13/cobra on 4-Jan-2021
