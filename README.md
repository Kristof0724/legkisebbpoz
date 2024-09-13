# legkisebbpoz
 var tomb = new int[5];
            Console.WriteLine("adj meg egy számot");
            for (int i = 0; i < tomb.Length; i++)
            {
                tomb[i] = int.Parse(Console.ReadLine());
            }
            Console.WriteLine(" a számok visszafelé");
            for (int i = 0; i < tomb.Length; i++)
            {
                Console.WriteLine(tomb[tomb.Length-1-i]);
            }




            int min = 0;
            for (int i = 1; i < tomb.Length; i++)
            {
                if (tomb[i] < tomb[min])
                {
                    min = i;
                }
            }
            Console.WriteLine($"Legkisebb szám pozíciója: {min+1} , értéke: {tomb[min]}");
