//Property Validation

```C# 
// creating the Area property validation logic
public int Area
{
  get { return area; }
  set 
  { 
    if (value < 0) { area = 0; }
    else { area = value; }
  }
}

// In Program.cs when we call the class

Forest f = new Forest();
// set() is called
f.Area = -1; 
// get() is called; prints 0
Console.WriteLine(f.Area);
```
