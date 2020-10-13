import java.util.*;
class A{
	public static void main(String []args){
		Scanner sc = new Scanner(System.in);
		
		System.out.println("这是一个回形字符串判断程序");
		System.out.println("请输入一个小于100字节的字符串（允许带空格）：");
		
		String a = sc.nextLine(); //允许输入带空格字符串的格式
		char b[] = new char[100]; //栈
		int n = a.length() , i = 0, j = 0;     //将字符串a的长度赋值给n
		
		while(true){
			if(j >= n){
				break;
			}
			else if(a.charAt(j) == ' '){
				j++;
			}
			else{
				b[i++] = a.charAt(j++);
			}
		}
		System.out.print("\n去掉空格后字符串为：");
		for(j = 0; j <= i; j++){
			System.out.print(b[j]);
		}
		j = 0; i--; n = 1; //j从前往后，i从后往前,n判断是否为回形字符串
		while(j <= i){
			if(b[j++] != b[i--]){
				n = 0;
			}
		}
		if(n == 1){
			System.out.printf("\n\n###这是回形字符串###\n");
		}
		else{
			System.out.printf("\n\n###这不是回形字符串###\n");
		}
	}
}
