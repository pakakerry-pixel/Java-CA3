public class Solution {
    public int lengthOfLastWord(String s) {
        int length = 0;
        int i = s.length() - 1;

        while (i >= 0 && s.charAt(i) == ' ') {
            i--;
        }

     
        while (i >= 0 && s.charAt(i) != ' ') {
            length++;
            i--;
        }

        return length;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        System.out.println(solver.lengthOfLastWord("Hello World"));                 // 5
        System.out.println(solver.lengthOfLastWord("   fly me   to   the moon  ")); // 4
        System.out.println(solver.lengthOfLastWord("luffy is still joyboy"));      // 6
    }
}
