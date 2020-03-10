# Ansible Role: Couchbase

## Requirements

N/A

## Role Variables

defaults/main.yml

## Dependencies

None.

## Example Inventory

```ini
couchbase-1.domain.tld ansible_host=*ip*
couchbase-2.domain.tld ansible_host=*ip*
couchbase-3.domain.tld ansible_host=*ip*

[couchbase_all]
couchbase-1.domain.tld
couchbase-2.domain.tld
couchbase-3.domain.tld

[couchbase_data_service]
couchbase-1.domain.tld
couchbase-2.domain.tld
couchbase-3.domain.tld

[couchbase_index_service]
couchbase-3.domain.tld

[couchbase_query_service]
couchbase-3.domain.tld

[couchbase_fts_service]
couchbase-3.domain.tld
```

## Example Playbook

```yaml
- hosts: all
  roles:
    - ansible-couchbase
```

## License

MIT
