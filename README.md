# ActionKit

Welcome to ActionKit

ActionKit is a general-purpose framework for expressing Actions, with a focus on distributed architectures.

ActionKit contains features built with C# / .Net Core and Typescript and aims to be as dependency-free as possible.

**Action** defined as:
```iecst 
1a : A thing done, DEED
1b : The accomplishment of a thing usually over a period of time, in stages, or with The possibility of repetition
1c : *Actions* plural
1d : INITIATIVE, ENTERPRISE

2 : An act of will
```

## A thing done

Getting something done in a safe, predictable, and fault-tolerant way is **not** straightforward. ActionKit is an opinionated look at *one of the great **many** ways* to ensure that things get done in a world of increasing technical complexity.

ActionKit focuses on:

- Useability
- Visibility
- Scalability

### Useability

*ActionKit should be usable for developers of most experience levels* with an understanding that distributed Actions is an advanced concept and may require additional training to fully utilize in production environments.

ActionKit provides the following:

- [actionKit](https://www.npmjs.com/package/actionkit) - NPM-distributed Typescript/JS  library to manage and invoke actions through a gateway.
- [Action.Kit](https://github.com/EthersoftOpen/Action.Kit) - .Net Standard Library
- [ActionGateway](https://github.com/EthersoftOpen/Action.Kit.Gateway) - .Net Core-powered Web Gateway reference implementation
- [Actor](https://github.com/EthersoftOpen/Action.Kit.Actor) - .Net Core based Event Listener that performs actions. Requires an ActionGateway.

### Visibility

ActionKit aims to enable complete visibility into it's structure at development time: Sourcemaps, comments, documentation.

In addition, ActionGateway/Actor will provide event-based telemetry at run time to allow easy ingestion of data into existing telemetry pipelines. This integration will allow DevOps teams to rapidly integrate ActionKit-powered applications into their platform.

ActionGateway supports the following:

- [WebHook Registration/Notification](README.md) - Have the ActionGateway message configured endpoints on specific events.
- ELK
- More

### Scalability

ActionKit should be as usable for the Application Developer as for the Platform Architect. ActionKit should be built responsibly so that developers utilizing our code need only worry about optimizing theirs. Unfortunately some pieces of ActionKit utilize things like the Network and Storage that are of limited resource. In those applications, we fall back on **Visibility** and surface the appropriate metrics to the consumer so that resources can be allocated.

**ActionGateway** features the following Scale-Out features for enterprise deployments:

- Distributed Action Repository - Easily distribute your Actions to Actors
- Transaction-based Action Tracing - Modeled log and trace information for your Actions
- Optional database-backed datastore
 

### License

This project is licensed under the [MIT License](LICENSE).

### Citations
1. Miram Webster [https://www.merriam-webster.com/dictionary/action]