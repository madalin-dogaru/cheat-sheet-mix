```C#
    public string Name
    { get; set; }
```
The above automatic property will replace: 
```
public string name;
public string Name
    {
      get { return name; }
      set { name = value; }
    }
```
