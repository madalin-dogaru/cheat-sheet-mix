```C#
// Program.cs - instantiating the class and initializing the fields from the main()
using System;

namespace BasicClasses
{
  class Program
  {
    static void Main(string[] args)
    {
      Forest f = new Forest();
      f.name = "Congo";
      f.trees = 0;
      f.age = 0;
      f.biome = "Tropical";
      
      Console.WriteLine(f.name);
    }
  }
}



// Forest.cs - declaring the class and its fields(class members) in its own file
using System;

namespace BasicClasses
{
  class Forest
  {
    public string name;
    public int trees;
    public int age;
    public string biome;
    
  }

}
