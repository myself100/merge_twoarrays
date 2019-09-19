# merge_twoarrays

package elclipse;
import java.util.*;
public class Merge {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {1,3,5,7,9};
		int b[]= {2,4,6,8,10};
		int ans[]= new int [a.length+b.length];   /// building array of size a and b
		int i=0,j=0,k=0;
        while(i<a.length && j<b.length) {
        	if(a[i]<b[j]) {
        		ans[k++]=a[i++];
        	}
        	else {
        		ans[k++]=b[j++];
        	}
        }
        while(i<a.length) {                ////
        	ans[k++]=a[i++];
        }
        while(j<b.length) {
        	ans[k++]=b[j++];
        }
        System.out.print(Arrays.toString(ans));
	}
}

