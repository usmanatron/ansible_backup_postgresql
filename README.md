# Ansible Role: Backup PostgreSQL Database

Backs up a PostgreSQL database daily.  Keeps the last 30 days of backups by default. Assumes the database is local to the machine.

## Requirements

None

## Role Variables

### Main Variables

| Name | Details |
| --- | --- |
| `parent_directory` | The full parent directory of where you want to store the backups. The rolw will add a `backups` directory to this location. |
| `database_name` | The name of the database to backup |
| `database_username` | The username to use to login to the database instance |
| `database_password` | The password to use to login to the database instance |

### Default Variables

| Name | Default Value | Details |
| --- | --- | --- |
| `retention_days` | `30` | Number of days to keep backups |

## License

MIT
