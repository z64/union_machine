# `union_machine`

Docker services for Union Machine.

## Running

```sh
docker-compose up -d
```

## Services

### `dev`

Container for programming and development.

VirtualBox should be configured to mount our drives with the following names:

Path  | Name
------|----------
P:\ | `P_DRIVE`
U:\ | `U_DRIVE`

See the `Dockerfile` for `dev` for more details.
