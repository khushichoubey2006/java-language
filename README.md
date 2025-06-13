import java.util.ArrayList;
import java.util.List;                

class GfG {
    public static List<Integer> spirallyTraverse(int[][] mat) {
        ArrayList<Integer> res = new ArrayList<>();
        int m = mat.length;
        int n = mat[0].length;
