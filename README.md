# gobadger

simple golang badgerDB api

## Feature

```
type DB interface {
	Incr(k string, by int64) (int64, error)
	Set(k, v string, ttl int) error
	MSet(data map[string]string) error
	Get(k string) (string, error)
	MGet(keys []string) []string
	Del(keys []string) error
	Scan(ScannerOpt ScannerOptions) error
	Size() int64
	GC() error
}
```
