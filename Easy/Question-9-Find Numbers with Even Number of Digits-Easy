public class Solution {
    public int findNumbers(int[] nums) {
        int count = 0;
        for (int num : nums) {
            
            int digits = (int) Math.log10(num) + 1;
            if (digits % 2 == 0) {
                count++;
            }
        }
        return count;
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        int[] nums1 = {12, 345, 2, 6, 7896};
        int[] nums2 = {555, 901, 482, 1771};

        System.out.println(solver.findNumbers(nums1)); // Output: 2
        System.out.println(solver.findNumbers(nums2)); // Output: 1
    }
}
