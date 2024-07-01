# Maximum-Product
This was a java project that I created as a part of my final for my AP Computer Science class.

For this program, I was tasked to find a subarray that has the largest product, given an integer array nums, and return the product. My initial approach was to simply use a for loop to iterate through the array list, multiplying the number at position i and i+1 every time. Then, I would add that product to a variable called max product if the product is greater than the value in max product. Though, this technique did not take into consideration the negative integers passed into the array list. After re-assessing my approach, I realized that I would need to adjust my approach depending on the number of negative integers in the array list. After creating a safety net to return 0 if the array list doesn’t have any numbers, I used a for loop to count the number of negative integers in the array list passed into the method. Then, I used if/else if statements to differentiate my approach by checking if the number of negative integers, stored in a variable named negs, is even or odd using the modulus operator. If the negatives are even, I continue as normal. I use a for loop to traverse the array list, and an if statement in the loop to check if the product of the numbers at position i and i+1 is greater than the current max product. If it is, I set max product and update my i to the next position using +1 and i+1 to its next position, which would be +2. Otherwise, if the number of negative integers is odd, I still start with a for loop to traverse the array list. Since the negative numbers would not cancel out as they do if they were even, I use a while loop to only conduct the same process I did if the negative numbers were even while the position at i is not a negative number. Otherwise, while the position at i is a negative number, I skip that number and break the loop. I used a separate method to check the program by creating a new array list and passing in the test case of [-2, 0, -1]. Then, I printed out the call to the method, passing in the array list created. 
