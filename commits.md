Commit conventions
===

Message format
---

We loosely follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/#specification). This is a template:

```
<type>(<scope>[/subscope]): <description>  

[<description>]

[<test instruction>]  

[<issue>]
```

Example:

> feature(loader): read weather from excel
>
> Ambient temperature used to be loaded from an H2 SQL script.  
> This is now loaded from an excel file.
>
> Run automated tests with `./gradlew :loader:test`
>
> To manually test this, use this version of the loader with the demo model   
> and observe that no H2 SQL scripts are necessary, but there is still weather data.
>
> Closes #4

The title has a soft limit at 50 characters.

There is no line limit for the body. You may choose to break text at 72 characters for readability.

Exemptions
---

Commits in a feature branch which will be squashed when merged do not need to conform to this format. The squashed commit however must conform to this format.
