import java.util.Arrays;

public class Solution {
    public void setZeroes(int[][] matrix) {
        int m = matrix.length;
        int n = matrix[0].length;

        boolean firstRowZero = false;
        boolean firstColZero = false;

        for (int i = 0; i < m; i++) {
            if (matrix[i][0] == 0) {
                firstColZero = true;
                break;
            }
        }

        for (int j = 0; j < n; j++) {
            if (matrix[0][j] == 0) {
                firstRowZero = true;
                break;
            }
        }

        for (int i = 1; i < m; i++) {
            for (int j = 1; j < n; j++) {
                if (matrix[i][j] == 0) {
                    matrix[i][0] = 0;
                    matrix[0][j] = 0;
                }
            }
        }

        for (int i = 1; i < m; i++) {
            for (int j = 1; j < n; j++) {
                if (matrix[i][0] == 0 || matrix[0][j] == 0) {
                    matrix[i][j] = 0;
                }
            }
        }

        if (firstRowZero) {
            for (int j = 0; j < n; j++) {
                matrix[0][j] = 0;
            }
        }

        if (firstColZero) {
            for (int i = 0; i < m; i++) {
                matrix[i][0] = 0;
            }
        }
    }

    public static void main(String[] args) {
        Solution solver = new Solution();

        int[][] matrix1 = {
            {1, 1, 1},
            {1, 0, 1},
            {1, 1, 1}
        };
        solver.setZeroes(matrix1);
        System.out.println(Arrays.deepToString(matrix1)); // Output: [[1, 0, 1], [0, 0, 0], [1, 0, 1]]

        int[][] matrix2 = {
            {0, 1, 2, 0},
            {3, 4, 5, 2},
            {1, 3, 1, 5}
        };
        solver.setZeroes(matrix2);
        System.out.println(Arrays.deepToString(matrix2)); // Output: [[0, 0, 0, 0], [0, 4, 5, 0], [0, 3, 1, 0]]
    }
}
