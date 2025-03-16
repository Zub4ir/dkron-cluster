# DKron

Pro Edition

## ACL

Remember to modify the rpc address if the needed.

```bash
# bootstrap
./dkron acl bootstrap --rpc-addr dkron-leader:6868

# create read.only
./dkron acl policy apply --name readonly --rules-file ./policies/readonly.json --rpc-addr dkron-leader:6868
./dkron acl token create --name read.only --type client --policy readonly --rpc-addr dkron-leader:6868

# list tokens
./dkron acl token list --rpc-addr dkron-leader:6868
```

## API

```shell
curl --header "Authorization: Bearer SECRET" http://localhost:8080/v1/jobs
```
