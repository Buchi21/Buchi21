- 👋 Hi, I’m Buchi
- 👀 In my free time i really like to code some stuff :)

## Performance Profiling

To enable performance profiling, start the agent with the `-profiling` configuration flag.

When enabled, the agent will generate two profiling files in its root directory:

- `cpu.pprof` – captures CPU usage
- `heap.pprof` – captures RAM/memory usage


### Visualize

You can visualize the profiling data using the `pprof` tool provided by the Go toolchain.

#### Command Syntax

```bash
go tool pprof -http=:<PORT> <Path-to-Agent-Binary> <Path-to-.pprof-File>
```

#### Example

```bash
go tool pprof -http=:8080 "C:\Program Files (x86)\Lywand Agent\bin\9.9.9\ly-agent.exe" "C:\Program Files (x86)\Lywand Agent\cpu.pprof"
```


