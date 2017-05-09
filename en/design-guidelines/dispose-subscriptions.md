# Dispose your subscriptions

http://www.introtorx.com/content/v1.0.10621.0/03_LifetimeManagement.html

```
this.WhenActivated(
    disposables =>
    {
        this.WhenAnyValue(...)
            .DisposeWith(disposables);
    });
```