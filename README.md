class sort{
  public static void insertSort(int array[]){
		int key,index;
		for(int i=0;i<array.length;i++){
			key=array[i];
			for(index=i-1;index>0&&array[index]>key;index--){
				array[index+1]=array[index];
			}
			array[index+1]=key;
		}
	}
}
public class SortTest {
	public static void main(String[] args){
		int array[]={2,6,9,34,18,3,48,16,29};
		sort.insertSort(array);
		System.out.print("直接插入排序的最终结果为:");
		for(int i:array){
			System.out.print(i+" ");
		}
	}
}
