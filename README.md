# -
随机出四则运算题，包括真假分数的四则运算


import java.util.Random;

public class szys
{
	public static void main(String args[])
	{
		for(int i=0;i<30;i++){
			int a1,a2,b1,b2,c,zf;
			a1=sjs(100);
			a2=sjs(100);
			b1=sjs(100);
			b2=sjs(100);
			c=sjs(4);
			zf=sjs(2);
			if(zf==0){
				if(c==0)
					System.out.println(a1+"+"+a2+"=  ");
				else if(c==1)
					System.out.println(a1+"-"+a2+"=  ");
				else if(c==2)
					System.out.println(a1+"*"+a2+"=  ");
				else if(c==3&&a2!=0)
					System.out.println(a1+"/"+a2+"=  ");
			}
			else if(zf==1){
				if(c==0)
					System.out.println(a1+"/"+a2+"   +  "+b1+"/"+b2+"=");
				else if(c==1)
					System.out.println(a1+"/"+a2+"   -  "+b1+"/"+b2+"=");
				else if(c==2)
					System.out.println(a1+"/"+a2+"   *  "+b1+"/"+b2+"=");
				else if(c==3&&a2!=0)
					System.out.println(a1+"/"+a2+"   /  "+b1+"/"+b2+"=");
				
			}
		}
	}
	public static int sjs(int i){
		Random a=new Random();
		int a1=a.nextInt (i);
		return a1;
	}
}
