//Property Validation
### Example 1
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

// In Program.cs when we try to set a value to the fields

Forest f = new Forest();
// set() is called
f.Area = -1; 
// get() is called; prints 0
Console.WriteLine(f.Area);
```

### Example 2
```C#
using System;

namespace BasicClasses
{
  class Forest
  {
    public string name;
    public int trees;
    public int age;
    public string biome;
    
    public string Name
    {
      get { return name; }
      set { name = value; }
    }
    
    public int Trees
    {
      get { return trees; }
      set { trees = value; }
    }
    
    public string Biome
    {
      get { return biome; }
      set
      {
        if (value == "Tropical" ||
            value == "Temperate" ||
            value == "Boreal")
        {
          biome = value;
        }
        else
        {
          biome = "Unknown";
        }
      }
    }
  }

}

// Program.cs or Main()
using System;

namespace BasicClasses
{
  class Program
  {
    static void Main(string[] args)
    {
      Forest f = new Forest();
      f.Name = "Congo";
      f.Trees = 0;
      f.age = 0;
      f.Biome = "Tropical";
      
      Console.WriteLine(f.Biome);
    }
  }
}
```
