```C#
public string Name
{ get; set; }
```
The above automatic property will replace the one bellow and and will do the same thing: 
```C#
public string name;
public string Name
    {
      get { return name; }
      set { name = value; }
    }
```
