# NANO-NOVEL
Nano Novel try

package NovelTry;

import java.util.Random;

public class FirstNovel {
	
	String Novel;
	static String [] NovWords;
	
	public FirstNovel(String novel){
		this.Novel = novel;
		this.NovWords = Novel.split(" ");
	}
	public static void switchUp(){
	String [] SwitchedUp = null;
		for(String word : NovWords){
			Random index = new Random();
			int Ind = index.nextInt(NovWords.length);
			SwitchedUp[Ind] = word;
		}
		System.out.println(SwitchedUp);
	}
	public static void main(String[] args){
		FirstNovel novel = new FirstNovel("Hello World");
		novel.switchUp();
	}
}

