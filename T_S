import java.io.BufferedReader;
import java.io.BufferedWriter;
import java.io.File;
import java.io.FileNotFoundException;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;

public class T9_Spelling {
	File ObF=new File("C:\\/Users\\/1531071\\/Documents\\/C-large-practice.in");
	FileReader ObR=null;
	BufferedReader brin=null;
	FileWriter ObW=null;
	BufferedWriter brout=null;
	int first_row;
	int iter=1;	
	int Sum;
	int internal_iter;
	int[] v=new int[2000];
	char[] c=new char[2000];
	String st="";
	String st_dc;
	String st_sd;
	public String decoder(char c)
	{
		if(c=='a')
		{
			st_dc="2";
		}else if(c=='b')
		{
			st_dc="22";
		}else if(c=='c')
		{
			st_dc="222";
		}else if(c=='d')
		{
			st_dc="3";
		}else if(c=='e')
		{
			st_dc="33";
		}else if(c=='f')
		{
			st_dc="333";
		}else if(c=='g')
		{
			st_dc="4";
		}else if(c=='h')
		{
			st_dc="44";
		}else if(c=='i')
		{
			st_dc="444";
		}else if(c=='j')
		{
			st_dc="5";
		}else if(c=='k')
		{
			st_dc="55";
		}else if(c=='l')
		{
			st_dc="555";
		}else if(c=='m')
		{
			st_dc="6";
		}else if(c=='n')
		{
			st_dc="66";
		}else if(c=='o')
		{
			st_dc="666";
		}else if(c=='p')
		{
			st_dc="7";
		}else if(c=='q')
		{
			st_dc="77";
		}else if(c=='r')
		{
			st_dc="777";
		}else if(c=='s')
		{
			st_dc="7777";
		}else if(c=='t')
		{
			st_dc="8";
		}else if(c=='u')
		{
			st_dc="88";
		}else if(c=='v')
		{
			st_dc="888";
		}else if(c=='w')
		{
			st_dc="9";
		}else if(c=='x')
		{
			st_dc="99";
		}else if(c=='y')
		{
			st_dc="999";
		}else if(c=='z')
		{
			st_dc="9999";
		}else if(c==' ')
		{
			st_dc="0";
		}
		return st_dc;	
	}
	public String space_detector(char x1,char x2)
	{
		if((x1=='a'|| x1=='b'|| x1=='c')&&(x2=='a'|| x2=='b'|| x2=='c'))
		{
			st_sd=" ";
		}else if((x1=='d'|| x1=='e'|| x1=='f')&&(x2=='d'|| x2=='e'|| x2=='f'))
		{
			st_sd=" ";
		}else if((x1=='g'|| x1=='h'|| x1=='i')&&(x2=='g'|| x2=='h'|| x2=='i'))
		{
			st_sd=" ";
		}else if((x1=='j'|| x1=='k'|| x1=='l')&&(x2=='j'|| x2=='k'|| x2=='l'))
		{
			st_sd=" ";
		}else if((x1=='m'|| x1=='n'|| x1=='o')&&(x2=='m'|| x2=='n'|| x2=='o'))
		{
			st_sd=" ";
		}else if((x1=='p'|| x1=='q'|| x1=='r' || x1=='s')&&(x2=='p'|| x2=='q'|| x2=='r' || x2=='s'))
		{
			st_sd=" ";
		}else if((x1=='t'|| x1=='u'|| x1=='v')&&(x2=='t'|| x2=='u'|| x2=='v'))
		{
			st_sd=" ";
		}else if((x1=='w'|| x1=='x'|| x1=='y' || x1=='z')&&(x2=='w'|| x2=='x'|| x2=='y' || x1=='z'))
		{
			st_sd=" ";
		}else
		{
			st_sd="";
		}

		return st_sd;	
	}


	public void  read() throws NumberFormatException, IOException
	{
		try {
			ObR=new FileReader(ObF);
			brin=new BufferedReader(ObR); 
			first_row=Integer.parseInt(brin.readLine());
			//System.out.println(first_row);

			while(iter<=first_row)
			{
				c=brin.readLine().toCharArray();
				new T9_Spelling().write(c);

				iter=iter+1;
			}

		} catch (FileNotFoundException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		} 


		//System.ou	t.println(i); 
	}
	public void  write(char[] c)
	{
		if(c.length==0)
		{
		st="0";	
		}else
		{
		for(int i=0; i<c.length;i++)
		{
			if(i==0)
			{
				st=st+(new T9_Spelling().decoder(c[i]));
			}else
			{
				st=st+(new T9_Spelling().space_detector(c[i-1],c[i]))+(new T9_Spelling().decoder(c[i]));
			}
		}
		}
	
			System.out.println(st); 
	}
	

	public static void main(String[] args) throws NumberFormatException, IOException {
		T9_Spelling obj=new T9_Spelling();
		obj.read();

	}

}
