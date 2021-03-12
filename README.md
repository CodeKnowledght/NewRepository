using System;

namespace Example_C_
{
	class Program 
	{
		public static void Main(string[] args)
		{
			int[][] n = new int[3][];
			n[0] = new int[] {1,2,3};
			n[1] = new int[] {4,5,6};
			n[2] = new int[] {7,8,9};
			foreach (int[] i in n)
			{
				foreach (int j in i)
				{
					Console.Write($"{j}\t");
				}
				Console.WriteLine();
			}
			Console.WriteLine();
			for (int i = 0; i < n.Length; ++i)
			{
				for (int j = 0; j < n[i].Length; ++j)
				{
					Console.Write($"{n[i][j]}\t");
				}
				Console.WriteLine();
			}
		}
	}
}
