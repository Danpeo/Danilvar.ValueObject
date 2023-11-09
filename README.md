# Value Object defined only by its value

Usage:

```
public class PowerLevel : ValueObject
{
    public int Value { get; }

    public PowerLevel(int value)
    {
        Value = value;
    }

    public override IEnumerable<object> GetAtomicValues()
    {
        yield return Value;
    }
}
```
