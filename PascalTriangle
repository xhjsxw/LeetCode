public class Solution {
    public List<List<Integer>> generate(int numRows) {
        if (numRows <= 0) {
			return  new ArrayList<List<Integer>>();
		}
		List<List<Integer>> result = new ArrayList<List<Integer>>();
		List<Integer> currentRow = new ArrayList<Integer>();
		List<Integer> previousList = new ArrayList<Integer>();
		currentRow.add(1);
		previousList = currentRow;
		result.add(currentRow);
		for (int i = 1; i < numRows; i++) {
			currentRow = new ArrayList<Integer>();
			currentRow.add(1);
			for (int j = 1; j < i; j++) {
				currentRow.add(previousList.get(j - 1) + previousList.get(j));
			}
			currentRow.add(1);
			result.add(currentRow);
			previousList = currentRow;
			currentRow = null;
		}
		currentRow = null;
		previousList = null;
		return result;
    }
}
