![image](https://hub.steampipe.io/images/plugins/turbot/hcloud-social-graphic.png)

# Hetzner Cloud Plugin for Steampipe

Use SQL to query servers, networks and more from Hetzner Cloud.

- **[Get started →](https://hub.steampipe.io/plugins/turbot/hcloud)**
- Documentation: [Table definitions & examples](https://hub.steampipe.io/plugins/turbot/hcloud/tables)
- Community: [Slack Channel](https://steampipe.io/community/join)
- Get involved: [Issues](https://github.com/turbot/steampipe-plugin-hcloud/issues)

## Quick start

Install the plugin with [Steampipe](https://steampipe.io):

```shell
steampipe plugin install hcloud
```

Run a query:

```sql
select
  id,
  name,
  created
from
  hcloud_server
```

## Developing

Prerequisites:

- [Steampipe](https://steampipe.io/downloads)
- [Golang](https://golang.org/doc/install)

Clone:

```sh
git clone https://github.com/turbot/steampipe-plugin-hcloud.git
cd steampipe-plugin-hcloud
```

Build, which automatically installs the new version to your `~/.steampipe/plugins` directory:

```
make
```

Configure the plugin:

```
cp config/* ~/.steampipe/config
vi ~/.steampipe/config/hcloud.spc
```

Try it!

```
steampipe query
> .inspect hcloud
```

Further reading:

- [Writing plugins](https://steampipe.io/docs/develop/writing-plugins)
- [Writing your first table](https://steampipe.io/docs/develop/writing-your-first-table)

## Contributing

Please see the [contribution guidelines](https://github.com/turbot/steampipe/blob/main/CONTRIBUTING.md) and our [code of conduct](https://github.com/turbot/steampipe/blob/main/CODE_OF_CONDUCT.md). All contributions are subject to the [Apache 2.0 open source license](https://github.com/turbot/steampipe-plugin-hcloud/blob/main/LICENSE).

`help wanted` issues:

- [Steampipe](https://github.com/turbot/steampipe/labels/help%20wanted)
- [Hetzner Cloud Plugin](https://github.com/turbot/steampipe-plugin-hcloud/labels/help%20wanted)
