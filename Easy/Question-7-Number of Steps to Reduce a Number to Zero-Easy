public class Solution {
    public int numberOfSteps(int num) {
        int steps = 0;

        while (num > 0) {
            if ((num & 1) == 0) {
                num >>= 1;
            } else {
                num--;    
            }
            steps++;
        }

        return steps;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        System.out.println(solver.numberOfSteps(14));  // Output: 6
        System.out.println(solver.numberOfSteps(8));   // Output: 4
        System.out.println(solver.numberOfSteps(123)); // Output: 12
    }
}
