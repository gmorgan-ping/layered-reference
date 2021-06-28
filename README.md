# layered-reference

In this example, we'll layer another profile onto the **getting-started/pingfederate** profile so that
we can manage the PingFederate license from within a separate profile.

View the [deply/values.yaml](deploy/values.yaml) file to see how multiple profiles can be specified. See Ping's DevOps [Documentation](https://devops.pingidentity.com/how-to/profilesLayered/) for additional information.

To deploy this example using helm

```sh
helm upgrade --install \
    <release-name> \
    pingidentity/ping-devops \
    -f https://raw.githubusercontent.com/gmorgan-ping/layered-reference/master/deploy/values.yaml
```
