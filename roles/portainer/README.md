# telerect-t-portainer
Portainer container for Telerec't

We recommend to use Portainer at a subdomain to your regular known domain like `portainer.example.com`.
If you don't have a subdomain to use which is usually the case for home servers with a purely local
installation of Portainer. In this case use a path prefix by setting `url_path_prefix: "/portainer"`

## Example configuration
This example configuration is a block you place in `group_vars/all.yml`:

```yaml
portainer:
  name: portainer
  admin_user: "admin"
  directory: "{{ docker_dir }}/portainer"
  domain: "homeserver.fritz.box"
  url_path_prefix: "/portainer"
  admin_password: "someSecretPasswordOfYourChoice"
```