 import java.util.ArrayList;
import java.util.List;                

class GfG {
    public static List<Integer> spirallyTraverse(int[][] mat) {
        ArrayList<Integer> res = new ArrayList<>();
        int m = mat.length;
        int n = mat[0].length;
        int top = 0, bottom = m - 1, left = 0, right = n - 1;
        while (top <= bottom && left <= right) {
            for (int i = left; i <= right; ++i) {
            }
            top++;
            // Print right column from top to bottom
            for (int i = top; i <= bottom; ++i) {
                res.add(mat[i][right]);
            }
            right--;
            }
            return res;
            }
         public static void main(String[] args) {
        int[][] mat = {{1, 2, 3, 4},
                {5, 6, 7, 8},
                {9, 10, 11, 12},
                {13, 14, 15, 16}};
         List<Integer> res = spirallyTraverse(mat);
        for (int ele : res) {
            System.out.print(ele + " ");
        }
    }





