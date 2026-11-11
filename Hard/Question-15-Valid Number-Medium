public class Solution {
    public boolean isNumber(String s) {
        boolean seenDigit = false;
        boolean seenDot = false;
        boolean seenExponent = false;

        for (int i = 0; i < s.length(); i++) {
            char ch = s.charAt(i);

            if (Character.isDigit(ch)) {
                seenDigit = true;
            } else if (ch == '+' || ch == '-') {
                if (i > 0 && s.charAt(i - 1) != 'e' && s.charAt(i - 1) != 'E') {
                    return false;
                }
            } else if (ch == '.') {
                if (seenDot || seenExponent) {
                    return false;
                }
                seenDot = true;
            } else if (ch == 'e' || ch == 'E') {
                if (seenExponent || !seenDigit) {
                    return false;
                }
                seenExponent = true;
                seenDigit = false;
            } else {
                return false;
            }
        }

        return seenDigit;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        System.out.println(solver.isNumber("0"));           // Output: true
        System.out.println(solver.isNumber("e"));           // Output: false
        System.out.println(solver.isNumber("."));           // Output: false
        System.out.println(solver.isNumber("2e10"));        // Output: true
        System.out.println(solver.isNumber("-123.456e789"));// Output: true
        System.out.println(solver.isNumber("99e2.5"));      // Output: false
        System.out.println(solver.isNumber("--6"));         // Output: false
    }
}
