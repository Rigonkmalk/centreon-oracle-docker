# Oracle Docker Compose

## Objective

Have a fast Oracle Instance for testing purpose.

### How-To

```bash
docker compose -f docker-compose up -d
```

### Usage from centreon_oracle.pl plugin

```bash
/usr/lib/centreon/plugins//centreon_oracle.pl --plugin=database::oracle::plugin --hostname='$HOSTNAME' --port='1521' --servicename='FREEPDB1' --username='system' --password='hibernate_orm_test'  --mode='connection-time' --warning='1000' --critical='5000'
```
