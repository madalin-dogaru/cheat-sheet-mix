// f1, f2, and f3 are out parameters, so they must be prefixed with `out`.

static void GetFavoriteFoods(out string f1, out string f2, out string f3)
{
  // We are assigning values to the parameters instead of using `return`.
  f1 = "Sushi";
  f2 = "Pizza";
  f3 = "Hamburgers";
}
 
static void Main()
{
  string food1;
  string food2;
  string food3;
  
  // Variables passed to out parameters must also be prefixed with `out`.
  GetFavoriteFoods(out food1, out food2, out food3);
  
  // After the method call, food1 = "Sushi", food2 = "Pizza", and food3 = "Hamburgers".
  Console.WriteLine($"My top 3 favorite foods are {food1}, {food2}, and {food3}");
}
