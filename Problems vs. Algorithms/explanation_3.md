To choose the digits of each of the two numbers, mergesort was used. For simplicity, the selection of digits is done after the array is sorted, by taking one digit at a time off the left part of the array (sorted by descending order), and alternating adding them to the right of the two result numbers.

The array was sorted by descending order to reflect the final two numbers. The left digits have to be larger than the right, to maximize each number. The order of which digit gets added to which number does not matter, as a continuous digits pair adds up to the same sum, and the maximum sum is requested. The important thing is that the biggest two digits end up on the beginning of the two result numbers, etc.

Time complexity is O(n logn) with n items in the array, because of the mergesort. The final iteration takes O(n) time so it does not contribute. Space complexity is O(n).