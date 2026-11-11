public class Solution {
    public double myPow(double x, int n) {
        long N = n;

        if (N < 0) {
            x = 1.0 / x;
            N = -N;
        }

        double result = 1.0;
        double currentProduct = x;

        while (N > 0) {
            if ((N & 1) == 1) {
                result *= currentProduct;
            }
            currentProduct *= currentProduct;
            N >>= 1;
        }

        return result;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        System.out.println(solver.myPow(2.00000, 10));  // Output: 1024.0
        System.out.println(solver.myPow(2.10000, 3));   // Output: 9.261000000000001
        System.out.println(solver.myPow(2.00000, -2));  // Output: 0.25
        System.out.println(solver.myPow(2.00000, -2147483648)); // Output: 0.0
    }
}
