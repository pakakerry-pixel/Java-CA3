public class Solution {
    public boolean isPowerOfTwo(int n) {
        return n > 0 && (n & (n - 1)) == 0;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        System.out.println(solver.isPowerOfTwo(1));   // true (2^0)
        System.out.println(solver.isPowerOfTwo(16));  // true (2^4)
        System.out.println(solver.isPowerOfTwo(3));   // false
        System.out.println(solver.isPowerOfTwo(0));   // false
        System.out.println(solver.isPowerOfTwo(-16)); // false
    }
}
