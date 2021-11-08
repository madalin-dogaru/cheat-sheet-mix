```C#
// Creating and initializing Arrays

using System;

namespace AccessingArrays
{
  class Program
  {
    static void Main(string[] args)
    {     
      string[] summerStrut;
      
      summerStrut = new string[] { "Juice", "Missing U", "Raspberry Beret", "New York Groove", "Make Me Feel", "Rebel Rebel", "Card", "Los Angeles" };
      
      int[] ratings = { 5, 4, 4, 3, 3, 5, 5, 4 };
         
      Console.WriteLine ($"You rated the song {summerStrut[1]} {ratings[1]} stars");
      
    }
  }
}

//Editing Arrays

using System;

namespace EditingArrays
{
  class Program
  {
    static void Main(string[] args)
    {     
      string[] summerStrut;
      
      summerStrut = new string[] { "Juice", "Missing U", "Raspberry Beret", "New York Groove", "Make Me Feel", "Rebel Rebel", "Card", "Los Angeles" };
      
      int[] ratings = { 5, 4, 4, 3, 3, 5, 5, 4 };
      summerStrut[7] = "coke";
      ratings[7] = 5;
      
      
    }
  }
}



// Sorting Arrays

using System;

namespace BuiltInMethods
{
  class Program
  {
    static void Main(string[] args)
    {     
      string[] summerStrut;
      
      summerStrut = new string[] { "Juice", "Missing U", "Raspberry Beret", "New York Groove", "Make Me Feel", "Rebel Rebel", "Card", "Los Angeles" };
      
      int[] ratings = { 5, 4, 4, 3, 3, 5, 5, 4 };
      
      int threeRating = Array.IndexOf(ratings, 3);
      Console.WriteLine($"Song number {threeRating + 1} is rated three stars.");
      
      string findName = Array.Find(summerStrut, song => song.Length > 10);
      
      Console.WriteLine($"The first song that has more than 10 characters in the title is {findName}.");
      
      Array.Sort(summerStrut);
      string firstSong = summerStrut[0];
      string lastSong = summerStrut[7];
      Console.WriteLine($"The first song in the playlist is now {firstSong}.");
      Console.WriteLine($"The last song in the playlist is now {lastSong}.");

    }
  }
}

// More predefined array methods

using System;

namespace DocumentationHunt
{
  class Program
  {
    static void Main(string[] args)
    {     
      string[] summerStrut;
      
      summerStrut = new string[] { "Juice", "Missing U", "Raspberry Beret", "New York Groove", "Make Me Feel", "Rebel Rebel", "Despacito", "Los Angeles" };
      
      int[] ratings = { 5, 4, 4, 3, 3, 5, 5, 4 };
      
      string[] summerStrutCopy = new string[8];
      
      Array.Copy(summerStrut, summerStrutCopy, 8);
      Console.WriteLine(summerStrutCopy[0]);
      
      Array.Reverse(summerStrut);
      Console.WriteLine(summerStrut[0]);
      Console.WriteLine(summerStrut[7]);
      
      Array.Clear(ratings, 0, ratings.Length);
      Console.WriteLine(ratings[0]);


    }
  }
}

```
