---
layout: reference
section: learn
title: GetCurrentEventGroup
permalink: /learn/ref/Microsoft.Coyote.Actors/IActorRuntime/GetCurrentEventGroup
---
# IActorRuntime.GetCurrentEventGroup method

Returns the current [`EventGroup`](../EventGroupType) of the actor with the specified id. Returns null if the id is not set, or if the [`ActorId`](../ActorIdType) is not associated with this runtime. During testing, the runtime asserts that the specified actor is currently executing.

```csharp
public EventGroup GetCurrentEventGroup(ActorId currentActorId)
```

| parameter | description |
| --- | --- |
| currentActorId | The id of the currently executing actor. |

## Return Value

The current EventGroup or null.

## See Also

* class [EventGroup](../EventGroupType)
* class [ActorId](../ActorIdType)
* interface [IActorRuntime](../IActorRuntimeType)
* namespace [Microsoft.Coyote.Actors](../IActorRuntimeType)
* assembly [Microsoft.Coyote](../../MicrosoftCoyoteAssembly)

<!-- DO NOT EDIT: generated by xmldocmd for Microsoft.Coyote.dll -->