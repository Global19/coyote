# Task.Wait method (1 of 5)

Waits for the task to complete execution.

```csharp
public void Wait()
```

## See Also

* class [Task](../Task.md)
* namespace [Microsoft.Coyote.Tasks](../Task.md)
* assembly [Microsoft.Coyote](../../Microsoft.Coyote.md)

---

# Task.Wait method (2 of 5)

Waits for the task to complete execution. The wait terminates if a cancellation token is canceled before the task completes.

```csharp
public void Wait(CancellationToken cancellationToken)
```

| parameter | description |
| --- | --- |
| cancellationToken | A cancellation token to observe while waiting for the task to complete. |

## See Also

* class [Task](../Task.md)
* namespace [Microsoft.Coyote.Tasks](../Task.md)
* assembly [Microsoft.Coyote](../../Microsoft.Coyote.md)

---

# Task.Wait method (3 of 5)

Waits for the task to complete execution within a specified number of milliseconds.

```csharp
public bool Wait(int millisecondsTimeout)
```

| parameter | description |
| --- | --- |
| millisecondsTimeout | The number of milliseconds to wait, or -1 to wait indefinitely. |

## Return Value

True if the task completed execution within the allotted time; otherwise, false.

## See Also

* class [Task](../Task.md)
* namespace [Microsoft.Coyote.Tasks](../Task.md)
* assembly [Microsoft.Coyote](../../Microsoft.Coyote.md)

---

# Task.Wait method (4 of 5)

Waits for the task to complete execution within a specified time interval.

```csharp
public bool Wait(TimeSpan timeout)
```

| parameter | description |
| --- | --- |
| timeout | A time span that represents the number of milliseconds to wait, or TimeSpan.FromMilliseconds(-1) to wait indefinitely. |

## Return Value

True if the task completed execution within the allotted time; otherwise, false.

## See Also

* class [Task](../Task.md)
* namespace [Microsoft.Coyote.Tasks](../Task.md)
* assembly [Microsoft.Coyote](../../Microsoft.Coyote.md)

---

# Task.Wait method (5 of 5)

Waits for the task to complete execution. The wait terminates if a timeout interval elapses or a cancellation token is canceled before the task completes.

```csharp
public bool Wait(int millisecondsTimeout, CancellationToken cancellationToken)
```

| parameter | description |
| --- | --- |
| millisecondsTimeout | The number of milliseconds to wait, or -1 to wait indefinitely. |
| cancellationToken | A cancellation token to observe while waiting for the task to complete. |

## Return Value

True if the task completed execution within the allotted time; otherwise, false.

## See Also

* class [Task](../Task.md)
* namespace [Microsoft.Coyote.Tasks](../Task.md)
* assembly [Microsoft.Coyote](../../Microsoft.Coyote.md)

<!-- DO NOT EDIT: generated by xmldocmd for Microsoft.Coyote.dll -->
