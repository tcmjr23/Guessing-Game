# Guessing-Game
This project requests your name, low and high values, and asks you to guess what number it chooses! 
Here are some key code samples:

# public static int getRandomNumber(int low, int high)
	{
		int rand = (int) (Math.random() * (high - low + 1)) + low;
		return rand;
	}
   
This method utilizes Math.random() which returns a number within the specified range (between low and high).

# public static String compareToSecret(int guessedNum, int secretNum)
	{
		String guessIs = "";
		if (guessedNum < secretNum)
			guessIs = "low";
		else
			guessIs = "high";
		return guessIs;
	}
 This method compares your guess to the secret number chosen at random. It then tells the user if it is too low, too high, or just right using if else statements.
  
# public static boolean inRange(int low, int high, int num)
	{
		if (low <= num && num <= high)
		{
			return true;
		}
		else
		{
			return false;
		}
	}
This method tests whether or not the user's guess is within the range specified by the passed low and high values. 
