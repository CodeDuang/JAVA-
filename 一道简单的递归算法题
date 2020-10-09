/*算法题：一个人赶着鸭子去每个村庄卖，每经过一个村子卖去所赶鸭子的一半又一只。这样他经过了七个村子后还剩两只鸭子，问他出发时共赶多少只鸭子？经过每个村子卖出多少只鸭子？
*/

/*分析：
设经过的村子为n (n = 0,1,2,...,7)，根据题目分析可知递归结束的出口: n = 7时，剩余鸭子数rest = 2;

分析递归体：从后向前推 n=7时 ，reset = 2， 由于每经过一个村子，卖去所赶鸭子的一半又一只，因此七个村子后剩余的鸭子数 rest[7] = rest[6] - (rest[6]/2 + 1)

反推rest[6] = (rest[7] + 1) * 2

最终递归体: (rest[n+1] + 1) * 2;

综上   n=7      rest=2

 0<=n<7     rest=(rest(n+1) + 1) * 2
 */

class A{
	public static void main(String args[]){
		System.out.println("鸭子一开始有"+sum(0));
		for(int i = 1; i <= 7 ;i++){
			System.out.println("经过第"+i+"个村庄卖去"+(sum(i-1) - sum(i))+"个，还剩"+sum(i)+"个");
		}
	}
	public static int sum(int n){
		return n == 7 ? 2 : (sum(n + 1) + 1) * 2;
	}
}
