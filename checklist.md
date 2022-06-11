# Make Cloud-native apps - checklist

- [ ] __Codebase__ - One codebase tracked in revision control, many deploys
- [ ] __Dependencies__ - Explicitly declare and isolate dependencies
- [ ] __Config__ - Store config in the environment
- [ ] __Backing services__ - Treat backing services as attached resources
- [ ] __Build, release, run__ - Strictly separate build and run stages
- [ ] __Processes__ - Execute the app as one or more stateless processes
- [ ] __Port binding__ - Export services via port binding
- [ ] __Concurrency__ - Scale out via the process model
- [ ] __Disposability__ - Maximize robustness with fast startup and graceful shutdown
- [ ] __Dev/prod parity__ - Keep development, staging, and production as similar as possible
- [ ] __Logs__ - Treat logs as event streams
- [ ] __Admin processes__ - Run admin/management tasks as one-off processes

## source
[https://12factor.net/](https://12factor.net/)