---
layout: reference
section: learn
title: StateMachine
permalink: /learn/ref/Microsoft.Coyote.Actors/StateMachineType
---
# StateMachine class

Type that implements a state machine actor. Inherit from this class to declare a custom actor with states, state transitions and event handlers.

```csharp
public abstract class StateMachine : Actor
```

## Public Members

| name | description |
| --- | --- |
| abstract class [State](StateMachineStateType) | Abstract class representing a state. |
| abstract class [StateGroup](StateMachineStateGroupType) | Abstract class used for representing a group of related states. |

## Protected Members

| name | description |
| --- | --- |
| [StateMachine](StateMachine/StateMachine)() | Initializes a new instance of the [`StateMachine`](StateMachineType) class. |
| [CurrentState](StateMachine/CurrentState) { get; } | Gets the Type of the current state. |
| override [OnEventHandledAsync](StateMachine/OnEventHandledAsync)(…) | Asynchronous callback that is invoked when the actor finishes handling a dequeued event, unless the handler of the dequeued event raised an event or caused the actor to halt (either normally or due to an exception). Unless this callback raises an event, the actor will either become idle or dequeue the next event from its inbox. |
| [RaiseEvent](StateMachine/RaiseEvent)(…) | Raises the specified [`Event`](../Microsoft.Coyote/EventType) at the end of the current action. |
| [RaiseGotoStateEvent](StateMachine/RaiseGotoStateEvent)(…) | Raise a special event that performs a goto state operation at the end of the current action. |
| [RaiseGotoStateEvent&lt;TState&gt;](StateMachine/RaiseGotoStateEvent)() | Raise a special event that performs a goto state operation at the end of the current action. |
| [RaiseHaltEvent](StateMachine/RaiseHaltEvent)() | Raises a [`HaltEvent`](HaltEventType) to halt the actor at the end of the current action. |
| [RaisePopStateEvent](StateMachine/RaisePopStateEvent)() | Raise a special event that performs a pop state operation at the end of the current action. |
| [RaisePushStateEvent](StateMachine/RaisePushStateEvent)(…) | Raise a special event that performs a push state operation at the end of the current action. |
| [RaisePushStateEvent&lt;TState&gt;](StateMachine/RaisePushStateEvent)() | Raise a special event that performs a push state operation at the end of the current action. |

## Remarks

See [State machines](/coyote/learn/programming-models/actors/state-machines) for more information.

## See Also

* class [Actor](ActorType)
* namespace [Microsoft.Coyote.Actors](../MicrosoftCoyoteActorsNamespace)
* assembly [Microsoft.Coyote](../MicrosoftCoyoteAssembly)

<!-- DO NOT EDIT: generated by xmldocmd for Microsoft.Coyote.dll -->